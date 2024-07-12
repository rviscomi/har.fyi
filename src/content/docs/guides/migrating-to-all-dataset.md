---
title: Migrate queries to `all` dataset
description: Assisting with query migration to the new dataset
---

New tables have been introduced in the HTTP Archive dataset, which are more efficient and easier to use. The `all` dataset contains all the data from the previous `pages`, `requests`, and other datasets. This guide will help you migrate your queries to the new dataset.

## Migrating to `all.pages`

### Page data schemas comparison

previously | `all.pages`
---|---
date in a table name | [`date`](/reference/tables/pages/#date)
client as `_TABLE_SUFFIX` | [`client`](/reference/tables/pages/#client)
`url` in `pages.YYYY_MM_DD_client` | [`page`](/reference/tables/pages/#page)
not available | [`is_root_page`](/reference/tables/pages/#is_root_page)
not available | [`root_page`](/reference/tables/pages/#root_page)
not available | [`rank`](/reference/tables/pages/#rank)
`$.testID` within `payload` column in `pages.YYYY_MM_DD_client`, `wptid` column in `summary_pages.YYYY_MM_DD_client` | [`wptid`](/reference/tables/pages/#wptid)
`payload`  in `pages.YYYY_MM_DD_client` | [`payload`](/reference/tables/pages/#payload)
`req*`, `resp*` and other in `summary_pages.YYYY_MM_DD_client` | [`summary`](/reference/tables/pages/#summary)
`$.CUSTOM_METRIC_NAME` within `payload` column in `pages.YYYY_MM_DD_client` | [`custom_metrics`](/reference/tables/pages/#custom_metrics)
`report` in `lighthouse.YYYY_MM_DD_client` | [lighthouse](/reference/tables/pages/#lighthouse)
`feature`, `type`, `id` in `blink_features.features` | `feature`, `type`, `id` in [`features`](/reference/tables/pages/#features)
`category`, `app`, `info` in `technologies.YYYY_MM_DD_client` | `categories`, `technology`, `info` in [`technologies`](/reference/tables/pages/#technologies)
not available | [`metadata`](/reference/tables/pages/#metadata)

### Page query updates

- From `blink_features.features` to `all.pages`.

    ```diff lang="sql"
    SELECT
    -  url,
    +  page,
    -  feature,
    +  features.feature,
    -  type,
    +  features.type,
    -  id
    +  features.id
    -FROM `httparchive.blink_features.features`
    +FROM `httparchive.all.pages`,
    +UNNEST (features) AS features
    -WHERE yyyymmdd = DATE('2024-05-01')
    +WHERE date = '2024-06-01'
      AND client = 'desktop'
    +  AND is_root_page
    ```

- From `lighthouse.YYYY_MM_DD_client` to `all.pages`.

    :::note
    In the example query changes lead to query size increase: 4 TB -> 17 TB.
    :::

    ```diff lang="sql"
    SELECT
    -  url,
    +  page,
    -  JSON_QUERY(report, '$.audits.largest-contentful-paint.numericValue') AS LCP,
    +  JSON_QUERY(lighthouse, '$.audits.largest-contentful-paint.numericValue') AS LCP,
    -FROM `httparchive.lighthouse.2024_06_01_desktop`
    +FROM `httparchive.all.pages`
    +WHERE date = '2024-06-01'
    +  AND client = 'desktop'
    +  AND is_root_page
    ```

- From `pages.YYYY_MM_DD_client` to `all.pages`.

    ```diff lang="sql"
    SELECT
    -  url,
    +  page,
    -  _TABLE_SUFFIX AS client,
    +  client,
    -  JSON_QUERY(payload, '$.testID') AS testID,
    +  wptid,
    -- JSON with the results of the custom metrics,
    -  JSON_QUERY(payload, '$._privacy') AS custom_metrics,
    +  JSON_QUERY(custom_metrics, '$.privacy') AS custom_metrics,
    -FROM `httparchive.pages.2022_06_01_*`
    +FROM `httparchive.all.pages`
    +WHERE date = '2022-06-01'
    +  AND is_root_page
    ```

- From `summary_pages.YYYY_MM_DD_client` to `all.pages`.

    :::note
    In the example query changes lead to query size increase: 194 MB -> 110 GB.
    :::

    ```diff lang="sql"
    SELECT
    -  numDomains,
    +  CAST(JSON_VALUE(summary, '$.numDomains') AS INT64) AS numDomains,
      COUNT(0) pages,
    -  ROUND(AVG(reqTotal),2) avg_requests,
    +  ROUND(AVG(CAST(JSON_VALUE(summary, '$.reqTotal') AS INT64)),2) as avg_requests,
    -FROM `httparchive.summary_pages.2024_06_01_desktop`
    +FROM `httparchive.all.pages`
    +WHERE date = '2024-06-01'
    +  AND client = 'desktop'
    +  AND is_root_page
    GROUP BY
      numDomains
    HAVING
      pages > 1000
    ORDER BY
      numDomains ASC
    ```

- From `technologies.YYYY_MM_DD_client` to `all.pages`.

    :::note
    In the example query changes lead to query size increase: 6 GB -> 27 GB.
    :::

    ```diff lang="sql"
    SELECT
    -  url,
    +  page,
    -  category,
    +  technologies.categories,
    -  app,
    +  technologies.technology,
    -  info
    +  technologies.info
    -FROM `httparchive.technologies.2024_06_01_desktop`
    +FROM `httparchive.all.pages`,
    +UNNEST (technologies) AS technologies
    +WHERE date = '2024-06-01'
    +  AND client = 'desktop'
    +  AND is_root_page
    ```

## Migrating to `all.requests`

### Request data schemas comparison

previously | `all.requests`
---|---
date in a table name | [`date`](/reference/tables/requests/#date)
client as `_TABLE_SUFFIX` | [`client`](/reference/tables/requests/#client)
`page` in `requests.YYYY_MM_DD_client` | [`page`](/reference/tables/requests/#page)
not available | [`is_root_page`](/reference/tables/requests/#is_root_page)
not available | [`root_page`](/reference/tables/requests/#root_page)
`url` in `requests.YYYY_MM_DD_client` | [`url`](/reference/tables/requests/#url)
`firstHtml` in `summary_requests.YYYY_MM_DD_client` | [`is_main_document`](/reference/tables/requests/#is_main_document)
`type` in `summary_requests.YYYY_MM_DD_client` | [`type`](/reference/tables/requests/#type)
`$._index` within `payload` in `requests.YYYY_MM_DD_client` | [`index`](/reference/tables/requests/#index)
`payload` column in `requests.YYYY_MM_DD_client` | [`payload`](/reference/tables/requests/#payload)
`req*`, `resp*` and other in `summary_requests.YYYY_MM_DD_client` | [`summary`](/reference/tables/requests/#summary)
`req_*` and `reqOtherHeaders` in `almanac.requests` | [`request_headers`](/reference/tables/requests/#request_headers)
`resp_*` and `respOtherHeaders` in `almanac.requests` | [`response_headers`](/reference/tables/requests/#response_headers)
`body` in `response_bodies.YYYY_MM_DD_client` | [`response_body`](/reference/tables/requests/#response_body)

### Request query updates

- From `almanac.requests` to `all.requests`.

    ```diff lang="sql"
    SELECT
    -  LOWER(JSON_VALUE(request_headers, '$.name')) AS header_name,
    +  LOWER(request_headers.name) AS header_name,
    -  JSON_VALUE(request_headers, '$.value') AS header_value,
    +  request_headers.value AS header_value,
    -FROM `httparchive.almanac.requests`,
    +FROM `httparchive.all.requests`,
    -UNNEST(JSON_QUERY_ARRAY(request_headers)) AS request_headers
    +UNNEST(request_headers) AS request_headers
    WHERE date = '2024-06-01'
      AND client = 'desktop'
    -  AND firstHtml
    +  AND is_main_document
    +  AND is_root_page
    ```

- FROM `requests.YYYY_MM_DD_client` to `all.requests`.

    ```diff lang="sql"
    SELECT
      page,
      url,
    -  JSON_VALUE(payload, '$.response.content.mimeType') AS mimeType,
    +  JSON_VALUE(summary, '$.mimeType') AS mimeType,
    -  CAST(JSON_VALUE(payload, '$.response.bodySize') AS INT64) AS respBodySize,
    +  CAST(JSON_VALUE(summary, '$.respBodySize') AS INT64) AS respBodySize,
    -FROM `httparchive.requests.2024_06_01_desktop`
    +FROM `httparchive.all.requests`
    +WHERE date = '2024-06-01'
    +  AND client = 'desktop'
    +  AND is_root_page
    ```

- From `response_bodies.YYYY_MM_DD_client` to `all.requests`.

    :::note
    In the example query changes lead to query size increase: 40 TB -> 174 TB.
    :::

    ```diff lang="sql"
    SELECT
      page,
      url,
      BYTE_LENGTH(response_body) AS bodySize
    -FROM `httparchive.response_bodies.2024_06_01_desktop`
    +FROM `httparchive.all.requests`
    +WHERE date = '2024-06-01'
    +  AND client = 'desktop'
    +  AND is_root_page
    ```

- From `summary_requests.YYYY_MM_DD_client` to `all.requests`.

    :::note
    In the example query changes lead to query size increase: 8 GB -> 10 TB.
    :::

    ```diff lang="sql"
    SELECT
    -  ROUND(respBodySize/1024/100)*100 AS responseSize100KB,
    +  ROUND(CAST(JSON_VALUE(summary, '$.respBodySize') AS INT64)/1024/100)*100 AS responseSize100KB,
      COUNT(0) requests,
    -FROM `httparchive.summary_requests.2024_06_01_desktop`
    +FROM `httparchive.all.requests`
    +WHERE date = '2024-06-01'
    +  AND client = 'desktop'
    +  AND is_root_page
    GROUP BY responseSize100KB
    HAVING responseSize100KB > 0
    ORDER BY responseSize100KB ASC
    ```