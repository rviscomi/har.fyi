---
title: Request summary struct
description: Reference docs for the request summary struct
---

_Appears in: [`requests` table](/reference/tables/requests/#summary)_\
_As: `summary`_

JSON-encoded summarization of request data.

Here's an example of the decoded object:

```json
{
    "_cdn_provider": "Edgecast",
    "_gzip_save": 0,
    "expAge": 604800,
    "ext": "",
    "format": "",
    "method": "GET",
    "mimeType": "text/html",
    "redirectUrl": null,
    "reqBodySize": null,
    "reqCookieLen": 0,
    "reqHeadersSize": 683,
    "respBodySize": 648,
    "respCookieLen": 0,
    "respHeadersSize": 376,
    "respHttpVersion": "HTTP/2",
    "respSize": 648,
    "status": 200,
    "time": 285,
    "type": "html"
}
```

## Schema

### `time`

The total time taken for the request in milliseconds.

### `_cdn_provider`

The Content Delivery Network provider.

### `_gzip_save`

Bytes saved due to gzip compression.

### `method`

The HTTP method used for the request (e.g., "GET", "POST").

### `reqHeadersSize`

The size of the request headers in bytes.

### `reqBodySize`

The size of the request body in bytes.

### `reqCookieLen`

The length of the request cookies.

### `status`

The HTTP status code of the response.

### `respHttpVersion`

The HTTP version used in the response.

### `redirectUrl`

The URL to which the request was redirected.

### `respHeadersSize`

The size of the response headers in bytes.

### `respBodySize`

The size of the response body in bytes.

### `respSize`

The total size of the response in bytes.

### `mimeType`

The MIME type of the response.

### `ext`

The file extension of the requested resource.

### `format`

The format of the resource.

### `respCookieLen`

The length of the response cookies.

### `expAge`

The age of the cached response in seconds.
