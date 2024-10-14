---
title: Page summary struct
description: Reference docs for the page summary struct
---

_Appears in: [`pages` table](/reference/tables/pages/)_\
_As: `summary`_

JSON-encoded summarization of the page-level data.

Here's an example of the decoded object:

```json
{
    "SpeedIndex": 400,
    "TTFB": 232,
    "_connections": 1,
    "bytesAudio": 0,
    "bytesCss": 0,
    "bytesFlash": 0,
    "bytesFont": 0,
    "bytesGif": 0,
    "bytesHtml": 648,
    "bytesHtmlDoc": 648,
    "bytesImg": 648,
    "bytesJS": 0,
    "bytesJpg": 0,
    "bytesJson": 0,
    "bytesOther": 0,
    "bytesPng": 0,
    "bytesSvg": 0,
    "bytesText": 0,
    "bytesTotal": 1296,
    "bytesVideo": 0,
    "bytesWebp": 0,
    "bytesXml": 0,
    "cdn": "Edgecast",
    "crux": {
        "collectionPeriod": {
            "firstDate": {
                "day": 17,
                "month": 8,
                "year": 2024
            },
            "lastDate": {
                "day": 13,
                "month": 9,
                "year": 2024
            }
        },
        "key": {
            "formFactor": "DESKTOP",
            "url": "https://www.example.com/"
        },
        "metrics": {
            ...
        }
    },
    "fullyLoaded": 323,
    "gzipSavings": 0,
    "gzipTotal": 648,
    "maxDomainReqs": 1,
    "maxage0": 0,
    "maxage1": 0,
    "maxage30": 2,
    "maxage365": 0,
    "maxageMore": 0,
    "maxageNull": 0,
    "numCompressed": 2,
    "numDomElements": 12,
    "numDomains": 1,
    "numErrors": 1,
    "numGlibs": 0,
    "numHttps": 2,
    "numRedirects": 0,
    "onContentLoaded": 280,
    "onLoad": 320,
    "renderStart": 400,
    "reqAudio": 0,
    "reqCss": 0,
    "reqFlash": 0,
    "reqFont": 0,
    "reqGif": 0,
    "reqHtml": 1,
    "reqImg": 1,
    "reqJS": 0,
    "reqJpg": 0,
    "reqJson": 0,
    "reqOther": 0,
    "reqPng": 0,
    "reqSvg": 0,
    "reqText": 0,
    "reqTotal": 2,
    "reqVideo": 0,
    "reqWebp": 0,
    "reqXml": 0,
    "visualComplete": 400
}
```

## Schema

### `SpeedIndex`

The Speed Index score.

### `TTFB`

The time to first byte

### `_connections`

The number of connections.

### `bytesAudio`

The number of bytes for audio.

### `bytesCss`

The number of bytes for CSS.

### `bytesFlash`

The number of bytes for Flash.

### `bytesFont`

The number of bytes for font.

### `bytesGif`

The number of bytes for GIF.

### `bytesHtml`

The number of bytes for HTML.

### `bytesHtmlDoc`

The number of bytes for HTML document.

### `bytesImg`

The number of bytes for image.

### `bytesJS`

The number of bytes for JavaScript.

### `bytesJpg`

The number of bytes for JPG.

### `bytesJson`

The number of bytes for JSON.

### `bytesOther`

The number of bytes for other.

### `bytesPng`

The number of bytes for PNG.

### `bytesSvg`

The number of bytes for SVG.

### `bytesText`

The number of bytes for text.

### `bytesTotal`

The total number of bytes.

### `bytesVideo`

The number of bytes for video.

### `bytesWebp`

The number of bytes for WebP.

### `bytesXml`

The number of bytes for XML.

### `cdn`

The Content Delivery Network provider.

### `crux`

The crux data.

### `fullyLoaded`

The fully loaded time.

### `gzipSavings`

The bytes saved due to gzip compression.

### `gzipTotal`

The total bytes in gzip compression.

### `maxDomainReqs`

The maximum number of requests to a domain.

### `maxage0`

The maximum number of requests with a max-age of 0.

### `maxage1`

The maximum number of requests with a max-age of 1.

### `maxage30`

The maximum number of requests with a max-age of 30.

### `maxage365`

The maximum number of requests with a max-age of 365.

### `maxageMore`

The maximum number of requests with a max-age greater than 365.

### `maxageNull`

The maximum number of requests with a max-age of null.

### `numCompressed`

The number of compressed files.

### `numDomElements`

The number of DOM elements.

### `numDomains`

The number of domains.

### `numErrors`

The number of errors.

### `numGlibs`

The number of glibs.

### `numHttps`

The number of HTTPS requests.

### `numRedirects`

The number of redirects.

### `onContentLoaded`

The onContentLoaded time.

### `onLoad`

The onLoad time.

### `renderStart`

The renderStart time.

### `reqAudio`

The number of bytes for audio.

### `reqCss`

The number of bytes for CSS.

### `reqFlash`

The number of bytes for Flash.

### `reqFont`

The number of bytes for font.

### `reqGif`

The number of bytes for GIF.

### `reqHtml`

The number of bytes for HTML.

### `reqImg`

The number of bytes for image.

### `reqJS`

The number of bytes for JavaScript.

### `reqJpg`

The number of bytes for JPG.

### `reqJson`

The number of bytes for JSON.

### `reqOther`

The number of bytes for other.

### `reqPng`

The number of bytes for PNG.

### `reqSvg`

The number of bytes for SVG.

### `reqText`

The number of bytes for text.

### `reqTotal`

The total number of bytes for requests.

### `reqVideo`

The number of bytes for video.

### `reqWebp`

The number of bytes for WebP.

### `reqXml`

The number of bytes for XML.

### `visualComplete`

The visualComplete time.
