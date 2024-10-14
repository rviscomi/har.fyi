---
title: Request payload struct
description: Reference docs for the request payload struct
---

_Appears in: [`requests` table](/reference/tables/requests/#payload)_\
_As: `payload`_

JSON-encoded WebPageTest result data for a request.

**The actual schema of the WebPageTest result data is liable to change, depending on a request.**

Here's an example of the decoded object:

```json
{
    "_all_end": 234,
    "_all_ms": 233,
    "_all_start": 1,
    "_body_file": "001-44714C6F6C72B045136D19CA9894886A-body.txt",
    "_body_hash": "ea8fac7c65fb589b0d53560f5251f74f9e9b243478dcb6b3ea79b5e36449c8d9",
    "_bytesIn": 648,
    "_bytesOut": 2143,
    "_cacheControl": "max-age=604800",
    "_cache_time": null,
    "_cached": 0,
    "_cdn_provider": "Edgecast",
    "_certificates": [
        "-----BEGIN CERTIFICATE-----\nMIIHbjCCBlagAwIBAgIQB1vO8waJyK3fE+Ua9K/hhzANBgkqhkiG9w0BAQsFADBZ\nMQswCQYDVQQGEwJVUzEVMBMGA1UEChMMRGlnaUNlcnQgSW5jMTMwMQYDVQQDEypE\naWdpQ2VydCBHbG9iYWwgRzIgVExTIFJTQSBTSEEyNTYgMjAyMCBDQTEwHhcNMjQw\nMTMwMDAwMDAwWhcNMjUwMzAxMjM1OTU5WjCBljELMAkGA1UEBhMCVVMxEzARBgNV\nBAgTCkNhbGlmb3JuaWExFDASBgNVBAcTC0xvcyBBbmdlbGVzMUIwQAYDVQQKDDlJ\nbnRlcm5ldMKgQ29ycG9yYXRpb27CoGZvcsKgQXNzaWduZWTCoE5hbWVzwqBhbmTC\noE51bWJlcnMxGDAWBgNVBAMTD3d3dy5leGFtcGxlLm9yZzCCASIwDQYJKoZIhvcN\nAQEBBQADggEPADCCAQoCggEBAIaFD7sO+cpf2fXgCjIsM9mqDgcpqC8IrXi9wga/\n9y0rpqcnPVOmTMNLsid3INbBVEm4CNr5cKlh9rJJnWlX2vttJDRyLkfwBD+dsVvi\nvGYxWTLmqX6/1LDUZPVrynv/cltemtg/1Aay88jcj2ZaRoRmqBgVeacIzgU8+zmJ\n7236TnFSe7fkoKSclsBhPaQKcE3Djs1uszJs8sdECQTdoFX9I6UgeLKFXtg7rRf/\nhcW5dI0zubhXbrW8aWXbCzySVZn0c7RkJMpnTCiZzNxnPXnHFpwr5quqqjVyN/aB\nKkjoP04Zmr+eRqoyk/+lslq0sS8eaYSSHbC5ja/yMWyVhvMCAwEAAaOCA/IwggPu\nMB8GA1UdIwQYMBaAFHSFgMBmx9833s+9KTeqAx2+7c0XMB0GA1UdDgQWBBRM/tAS\nTS4hz2v68vK4TEkCHTGRijCBgQYDVR0RBHoweIIPd3d3LmV4YW1wbGUub3Jnggtl\neGFtcGxlLm5ldIILZXhhbXBsZS5lZHWCC2V4YW1wbGUuY29tggtleGFtcGxlLm9y\nZ4IPd3d3LmV4YW1wbGUuY29tgg93d3cuZXhhbXBsZS5lZHWCD3d3dy5leGFtcGxl\nLm5ldDA+BgNVHSAENzA1MDMGBmeBDAECAjApMCcGCCsGAQUFBwIBFhtodHRwOi8v\nd3d3LmRpZ2ljZXJ0LmNvbS9DUFMwDgYDVR0PAQH/BAQDAgWgMB0GA1UdJQQWMBQG\nCCsGAQUFBwMBBggrBgEFBQcDAjCBnwYDVR0fBIGXMIGUMEigRqBEhkJodHRwOi8v\nY3JsMy5kaWdpY2VydC5jb20vRGlnaUNlcnRHbG9iYWxHMlRMU1JTQVNIQTI1NjIw\nMjBDQTEtMS5jcmwwSKBGoESGQmh0dHA6Ly9jcmw0LmRpZ2ljZXJ0LmNvbS9EaWdp\nQ2VydEdsb2JhbEcyVExTUlNBU0hBMjU2MjAyMENBMS0xLmNybDCBhwYIKwYBBQUH\nAQEEezB5MCQGCCsGAQUFBzABhhhodHRwOi8vb2NzcC5kaWdpY2VydC5jb20wUQYI\nKwYBBQUHMAKGRWh0dHA6Ly9jYWNlcnRzLmRpZ2ljZXJ0LmNvbS9EaWdpQ2VydEds\nb2JhbEcyVExTUlNBU0hBMjU2MjAyMENBMS0xLmNydDAMBgNVHRMBAf8EAjAAMIIB\nfQYKKwYBBAHWeQIEAgSCAW0EggFpAWcAdABOdaMnXJoQwzhbbNTfP1LrHfDgjhuN\nacCx+mSxYpo53wAAAY1b0vxkAAAEAwBFMEMCH0BRCgxPbBBVxhcWZ26a8JCe83P1\nJZ6wmv56GsVcyMACIDgpMbEo5HJITTRPnoyT4mG8cLrWjEvhchUdEcWUuk1TAHYA\nfVkeEuF4KnscYWd8Xv340IdcFKBOlZ65Ay/ZDowuebgAAAGNW9L8MAAABAMARzBF\nAiBdv5Z3pZFbfgoM3tGpCTM3ZxBMQsxBRSdTS6d8d2NAcwIhALLoCT9mTMN9OyFz\nIBV5MkXVLyuTf2OAzAOa7d8x2H6XAHcA5tIxY0B3jMEQQQbXcbnOwdJA9paEhvu6\nhzId/R43jlAAAAGNW9L8XwAABAMASDBGAiEA4Koh/VizdQU1tjZ2E2VGgWSXXkwn\nQmiYhmAeKcVLHeACIQD7JIGFsdGol7kss2pe4lYrCgPVc+iGZkuqnj26hqhr0TAN\nBgkqhkiG9w0BAQsFAAOCAQEABOFuAj4N4yNG9OOWNQWTNSICC4Rd4nOG1HRP/Bsn\nrz7KrcPORtb6D+Jx+Q0amhO31QhIvVBYs14gY4Ypyj7MzHgm4VmPXcqLvEkxb2G9\nQv9hYuEiNSQmm1fr5QAN/0AzbEbCM3cImLJ69kP5bUjfv/76KB57is8tYf9sh5ik\nLGKauxCM/zRIcGa3bXLDafk5S2g5Vr2hs230d/NGW1wZrE+zdGuMxfGJzJP+DAFv\niBfcQnFg4+1zMEKcqS87oniOyG+60RMM0MdejBD7AS43m9us96Gsun/4kufLQUTI\nFfnzxLutUV++3seshgefQOy5C/ayi8y1VTNmujPCxPCi6Q==\n-----END CERTIFICATE-----\n",
        "-----BEGIN CERTIFICATE-----\nMIIEyDCCA7CgAwIBAgIQDPW9BitWAvR6uFAsI8zwZjANBgkqhkiG9w0BAQsFADBh\nMQswCQYDVQQGEwJVUzEVMBMGA1UEChMMRGlnaUNlcnQgSW5jMRkwFwYDVQQLExB3\nd3cuZGlnaWNlcnQuY29tMSAwHgYDVQQDExdEaWdpQ2VydCBHbG9iYWwgUm9vdCBH\nMjAeFw0yMTAzMzAwMDAwMDBaFw0zMTAzMjkyMzU5NTlaMFkxCzAJBgNVBAYTAlVT\nMRUwEwYDVQQKEwxEaWdpQ2VydCBJbmMxMzAxBgNVBAMTKkRpZ2lDZXJ0IEdsb2Jh\nbCBHMiBUTFMgUlNBIFNIQTI1NiAyMDIwIENBMTCCASIwDQYJKoZIhvcNAQEBBQAD\nggEPADCCAQoCggEBAMz3EGJPprtjb+2QUlbFbSd7ehJWivH0+dbn4Y+9lavyYEEV\ncNsSAPonCrVXOFt9slGTcZUOakGUWzUb+nv6u8W+JDD+Vu/E832X4xT1FE3LpxDy\nFuqrIvAxIhFhaZAmunjZlx/jfWardUSVc8is/+9dCopZQ+GssjoP80j812s3wWPc\n3kbW20X+fSP9kOhRBx5Ro1/tSUZUfyyIxfQTnJcVPAPooTncaQwywa8WV0yUR0J8\nosicfebUTVSvQpmowQTCd5zWSOTOEeAqgJnwQ3DPP3Zr0UxJqyRewg2C/Uaoq2yT\nzGJSQnWS+Jr6Xl6ysGHlHx+5fwmY6D36g39HaaECAwEAAaOCAYIwggF+MBIGA1Ud\nEwEB/wQIMAYBAf8CAQAwHQYDVR0OBBYEFHSFgMBmx9833s+9KTeqAx2+7c0XMB8G\nA1UdIwQYMBaAFE4iVCAYlebjbuYP+vq5Eu0GF485MA4GA1UdDwEB/wQEAwIBhjAd\nBgNVHSUEFjAUBggrBgEFBQcDAQYIKwYBBQUHAwIwdgYIKwYBBQUHAQEEajBoMCQG\nCCsGAQUFBzABhhhodHRwOi8vb2NzcC5kaWdpY2VydC5jb20wQAYIKwYBBQUHMAKG\nNGh0dHA6Ly9jYWNlcnRzLmRpZ2ljZXJ0LmNvbS9EaWdpQ2VydEdsb2JhbFJvb3RH\nMi5jcnQwQgYDVR0fBDswOTA3oDWgM4YxaHR0cDovL2NybDMuZGlnaWNlcnQuY29t\nL0RpZ2lDZXJ0R2xvYmFsUm9vdEcyLmNybDA9BgNVHSAENjA0MAsGCWCGSAGG/WwC\nATAHBgVngQwBATAIBgZngQwBAgEwCAYGZ4EMAQICMAgGBmeBDAECAzANBgkqhkiG\n9w0BAQsFAAOCAQEAkPFwyyiXaZd8dP3A+iZ7U6utzWX9upwGnIrXWkOH7U1MVl+t\nwcW1BSAuWdH/SvWgKtiwla3JLko716f2b4gp/DA/JIS7w7d7kwcsr4drdjPtAFVS\nslme5LnQ89/nD/7d+MS5EHKBCQRfz5eeLjJ1js+aWNJXMX43AYGyZm0pGrFmCW3R\nbpD0ufovARTFXFZkAdl9h6g4U5+LXUZtXMYnhIHUfoyMo5tS58aI7Dd8KvvwVVo4\nchDYABPPTHPbqjc1qCmBaZx2vN4Ye5DUys/vZwP9BFohFrH/6j/f3IL16/RZkiMN\nJCqVJUzKoZHm1Lesh3Sz8W2jmdv51b2EQJ8HmA==\n-----END CERTIFICATE-----\n"
    ],
    "_chunks": [
        {
            "bytes": 648,
            "inflated": 1256,
            "ts": 234
        }
    ],
    "_connect_end": 93,
    "_connect_ms": 33,
    "_connect_start": 60,
    "_contentEncoding": "gzip",
    "_contentType": "text/html",
    "_created": 8,
    "_dns_end": 60,
    "_dns_info": {
        "results": {
            "aliases": [
                "www.example.com"
            ],
            "canonical_names": [
                "www.example.com"
            ],
            "endpoint_metadatas": [],
            "expiration": "13370780176732624",
            "host_ports": [],
            "hostname_results": [],
            "ip_endpoints": [
                {
                    "endpoint_address": "93.184.215.14",
                    "endpoint_port": 0
                }
            ],
            "text_records": []
        },
        "secure": false,
        "transactions_needed": [
            {
                "dns_query_type": "A"
            },
            {
                "dns_query_type": "HTTPS"
            }
        ]
    },
    "_dns_ms": 59,
    "_dns_start": 1,
    "_documentURL": "https://www.example.com/",
    "_download_end": 234,
    "_download_ms": 2,
    "_download_start": 232,
    "_expires": "Sun, 22 Sep 2024 03:21:43 GMT",
    "_final_base_page": true,
    "_frame_id": "E021D0149DE3689992ECE4DF4B0ECA38",
    "_full_url": "https://www.example.com/",
    "_gzip_save": 0,
    "_gzip_total": 648,
    "_host": "www.example.com",
    "_http2_server_settings": {
        "SETTINGS_DEPRECATE_HTTP2_PRIORITIES": 0,
        "SETTINGS_ENABLE_PUSH": 0,
        "SETTINGS_HEADER_TABLE_SIZE": 4096,
        "SETTINGS_INITIAL_WINDOW_SIZE": 1048576,
        "SETTINGS_MAX_CONCURRENT_STREAMS": 100,
        "SETTINGS_MAX_FRAME_SIZE": 16384,
        "SETTINGS_MAX_HEADER_LIST_SIZE": 16384
    },
    "_http2_stream_dependency": 0,
    "_http2_stream_exclusive": 1,
    "_http2_stream_id": 1,
    "_http2_stream_weight": 256,
    "_id": "44714C6F6C72B045136D19CA9894886A",
    "_image_save": null,
    "_image_total": null,
    "_index": 0,
    "_initial_priority": "Highest",
    "_initiator": "",
    "_initiator_column": "",
    "_initiator_line": "",
    "_initiator_type": "script",
    "_ip_addr": "93.184.215.14",
    "_is_base_page": true,
    "_is_secure": 1,
    "_load_end": 234,
    "_load_ms": 43,
    "_load_start": 191,
    "_load_start_float": 191.000079,
    "_method": "GET",
    "_minify_save": null,
    "_minify_total": null,
    "_netlog_id": 79,
    "_number": 1,
    "_objectSize": 648,
    "_objectSizeUncompressed": 1256,
    "_priority": "Highest",
    "_protocol": "HTTP/2",
    "_raw_id": "44714C6F6C72B045136D19CA9894886A",
    "_request_id": "44714C6F6C72B045136D19CA9894886A",
    "_request_type": "Document",
    "_responseCode": 200,
    "_run": 1,
    "_score_cache": -1,
    "_score_cdn": 100,
    "_score_combine": -1,
    "_score_compress": -1,
    "_score_cookies": -1,
    "_score_etags": -1,
    "_score_gzip": 100,
    "_score_keep-alive": 100,
    "_score_minify": -1,
    "_securityDetails": {
        "certificateId": 0,
        "certificateTransparencyCompliance": "compliant",
        "cipher": "AES_256_GCM",
        "encryptedClientHello": false,
        "issuer": "DigiCert Global G2 TLS RSA SHA256 2020 CA1",
        "keyExchange": "",
        "keyExchangeGroup": "P-256",
        "protocol": "TLS 1.3",
        "sanList": [
            "www.example.org",
            "example.net",
            "example.edu",
            "example.com",
            "example.org",
            "www.example.com",
            "www.example.edu",
            "www.example.net"
        ],
        "serverSignatureAlgorithm": 2052,
        "signedCertificateTimestampList": [
            {
                "hashAlgorithm": "SHA-256",
                "logDescription": "Google 'Argon2025h1' log",
                "logId": "4E75A3275C9A10C3385B6CD4DF3F52EB1DF0E08E1B8D69C0B1FA64B1629A39DF",
                "origin": "Embedded in certificate",
                "signatureAlgorithm": "ECDSA",
                "signatureData": "3043021F40510A0C4F6C1055C61716676E9AF0909EF373F5259EB09AFE7A1AC55CC8C00220382931B128E472484D344F9E8C93E261BC70BAD68C4BE172151D11C594BA4D53",
                "status": "Verified",
                "timestamp": 1706642570340
            },
            {
                "hashAlgorithm": "SHA-256",
                "logDescription": "DigiCert Yeti2025 Log",
                "logId": "7D591E12E1782A7B1C61677C5EFDF8D0875C14A04E959EB9032FD90E8C2E79B8",
                "origin": "Embedded in certificate",
                "signatureAlgorithm": "ECDSA",
                "signatureData": "304502205DBF9677A5915B7E0A0CDED1A909333767104C42CC414527534BA77C77634073022100B2E8093F664CC37D3B21732015793245D52F2B937F6380CC039AEDDF31D87E97",
                "status": "Verified",
                "timestamp": 1706642570288
            },
            {
                "hashAlgorithm": "SHA-256",
                "logDescription": "DigiCert Nessie2025 Log",
                "logId": "E6D2316340778CC1104106D771B9CEC1D240F6968486FBBA87321DFD1E378E50",
                "origin": "Embedded in certificate",
                "signatureAlgorithm": "ECDSA",
                "signatureData": "3046022100E0AA21FD58B3750535B636761365468164975E4C2742689886601E29C54B1DE0022100FB248185B1D1A897B92CB36A5EE2562B0A03D573E886664BAA9E3DBA86A86BD1",
                "status": "Verified",
                "timestamp": 1706642570335
            }
        ],
        "subjectName": "www.example.org",
        "validFrom": 1706572800,
        "validTo": 1740873599
    },
    "_server_count": null,
    "_server_port": "443",
    "_server_rtt": null,
    "_socket": 86,
    "_socket_group": "https://www.example.com <https://example.com same_site>",
    "_ssl_end": 191,
    "_ssl_ms": 98,
    "_ssl_start": 93,
    "_tls_cipher_suite": 4866,
    "_tls_next_proto": "h2",
    "_tls_resumed": "False",
    "_tls_version": "TLS 1.3",
    "_ttfb_end": 232,
    "_ttfb_ms": 41,
    "_ttfb_start": 191,
    "_type": 3,
    "_url": "/",
    "cache": {},
    "pageref": "page_1_0_1",
    "request": {
        "bodySize": -1,
        "cookies": [],
        "headersSize": 683,
        "httpVersion": "HTTP/2",
        "method": "GET",
        "queryString": [],
        "url": "https://www.example.com/"
    },
    "response": {
        "bodySize": 648,
        "content": {
            "mimeType": "text/html",
            "size": 648
        },
        "cookies": [],
        "headersSize": 376,
        "httpVersion": "HTTP/2",
        "status": 200,
        "statusText": ""
    },
    "startedDateTime": "2024-09-15T03:21:43.105962",
    "time": 285,
    "timings": {
        "blocked": 52,
        "connect": 131,
        "dns": 59,
        "receive": 2,
        "send": 0,
        "ssl": 98,
        "wait": 41
    }
}
```

## Schema

| Field                                                | Type     | Description                                       |
| ---------------------------------------------------- | -------- | ------------------------------------------------- |
| `_all_end`                                           | `int`    | End time of all operations.                       |
| `_all_ms`                                            | `int`    | Total time taken for all operations.              |
| `_all_start`                                         | `int`    | Start time of all operations.                     |
| `_body_file`                                         | `string` | File containing the body of the request.          |
| `_bytesIn`                                           | `int`    | Number of bytes received.                         |
| `_bytesOut`                                          | `int`    | Number of bytes sent.                             |
| `_cache_time`                                        | `int`    | Cache time.                                       |
| `_cacheControl`                                      | `string` | Cache control header value.                       |
| `_cached`                                            | `int`    | Indicates if the request was cached (0 or 1).     |
| `_cdn_provider`                                      | `string` | CDN provider used.                                |
| `_certificates`                                      | `array`  | Certificates used.                                |
| `_chunks`                                            | `array`  | Array of chunks received.                         |
| `_chunks[].bytes`                                    | `int`    | Size of the chunk.                                |
| `_chunks[].inflated`                                 | `int`    | Size of the inflated chunk.                       |
| `_chunks[].ts`                                       | `int`    | Timestamp of the chunk.                           |
| `_connect_end`                                       | `int`    | Connection end time.                              |
| `_connect_ms`                                        | `int`    | Connection time in milliseconds.                  |
| `_connect_start`                                     | `int`    | Connection start time.                            |
| `_contentEncoding`                                   | `string` | Content encoding of the response.                 |
| `_contentType`                                       | `string` | Content type of the response.                     |
| `_created`                                           | `int`    | Creation time of the request.                     |
| `_dns_end`                                           | `int`    | DNS end time.                                     |
| `_dns_info`                                          | `object` | DNS information.                                  |
| `_dns_info.results.aliases`                          | `array`  | Aliases for the domain.                           |
| `_dns_info.results.canonical_names`                  | `array`  | Canonical names for the domain.                   |
| `_dns_info.results.endpoint_metadatas`               | `array`  | Endpoint metadata.                                |
| `_dns_info.results.expiration`                       | `string` | Expiration date of the DNS query.                 |
| `_dns_info.results.host_ports`                       | `array`  | Host ports.                                       |
| `_dns_info.results.hostname_results`                 | `array`  | Hostname results.                                 |
| `_dns_info.results.ip_endpoints[].endpoint_address`  | `string` | IP address of the endpoint.                       |
| `_dns_info.results.ip_endpoints[].endpoint_port`     | `int`    | Port of the endpoint.                             |
| `_dns_info.results.ip_endpoints`                     | `array`  | IP endpoints.                                     |
| `_dns_info.results.text_records`                     | `array`  | Text records.                                     |
| `_dns_info.results`                                  | `object` | Results of the DNS query.                         |
| `_dns_info.secure`                                   | `int`    | Indicates if the DNS query is secure.             |
| `_dns_info.transactions_needed[].dns_query_type`     | `string` | Type of DNS query.                                |
| `_dns_info.transactions_needed`                      | `array`  | Transactions needed for DNS query.                |
| `_dns_ms`                                            | `int`    | DNS lookup time in milliseconds.                  |
| `_dns_start`                                         | `int`    | DNS start time.                                   |
| `_documentURL`                                       | `string` | Document URL of the request.                      |
| `_download_end`                                      | `int`    | Download end time.                                |
| `_download_ms`                                       | `int`    | Download time in milliseconds.                    |
| `_download_start`                                    | `int`    | Download start time.                              |
| `_expires`                                           | `string` | Expiry date of the request.                       |
| `_final_base_page`                                   | `int`    | Indicates if the request is the final base page.  |
| `_frame_id`                                          | `string` | Frame ID where the request was made.              |
| `_full_url`                                          | `string` | Full URL of the request.                          |
| `_gzip_save`                                         | `int`    | Size saved due to gzip compression.               |
| `_gzip_total`                                        | `int`    | Total size of the gzip-compressed content.        |
| `_host`                                              | `string` | Host of the request.                              |
| `_http2_server_settings`                             | `object` | HTTP/2 server settings.                           |
| `_http2_stream_dependency`                           | `int`    | HTTP/2 stream dependency.                         |
| `_http2_stream_exclusive`                            | `int`    | HTTP/2 stream exclusivity.                        |
| `_http2_stream_id`                                   | `int`    | HTTP/2 stream ID.                                 |
| `_http2_stream_weight`                               | `int`    | HTTP/2 stream weight.                             |
| `_id`                                                | `string` | Unique identifier for the request.                |
| `_image_save`                                        | `int`    | Size saved due to image optimization.             |
| `_image_total`                                       | `int`    | Total size of images.                             |
| `_index`                                             | `int`    | Index of the request.                             |
| `_initial_priority`                                  | `string` | Initial priority of the request.                  |
| `_initiator_column`                                  | `string` | Column number of the initiator.                   |
| `_initiator_line`                                    | `string` | Line number of the initiator.                     |
| `_initiator_type`                                    | `string` | Type of initiator (e.g., script).                 |
| `_initiator`                                         | `string` | Initiator of the request.                         |
| `_ip_addr`                                           | `string` | IP address of the requested server.               |
| `_is_base_page`                                      | `int`    | Indicates if the request is the base page.        |
| `_is_secure`                                         | `int`    | Indicates if the request is secure (0 or 1).      |
| `_load_end`                                          | `int`    | Load end time.                                    |
| `_load_ms`                                           | `int`    | Load time in milliseconds.                        |
| `_load_start_float`                                  | `float`  | Precise start time of load.                       |
| `_load_start`                                        | `int`    | Start time of load in milliseconds.               |
| `_method`                                            | `string` | HTTP method used for the request.                 |
| `_minify_save`                                       | `int`    | Size saved due to minification.                   |
| `_minify_total`                                      | `int`    | Total size of minified content.                   |
| `_netlog_id`                                         | `int`    | Netlog ID.                                        |
| `_number`                                            | `int`    | Number of the request.                            |
| `_objectSize`                                        | `int`    | Size of the object received.                      |
| `_objectSizeUncompressed`                            | `int`    | Uncompressed size of the object received.         |
| `_priority`                                          | `string` | Priority of the request.                          |
| `_protocol`                                          | `string` | Protocol used for the request.                    |
| `_raw_id`                                            | `string` | Raw ID for the request.                           |
| `_request_id`                                        | `string` | Identifier for the original request.              |
| `_request_type`                                      | `string` | Type of the request (e.g., Document).             |
| `_responseCode`                                      | `int`    | HTTP response code.                               |
| `_run`                                               | `int`    | The run number of the test.                       |
| `_score_cache`                                       | `int`    | Cache score.                                      |
| `_score_cdn`                                         | `int`    | CDN score.                                        |
| `_score_combine`                                     | `int`    | Combine score.                                    |
| `_score_compress`                                    | `int`    | Compression score.                                |
| `_score_cookies`                                     | `int`    | Cookies score.                                    |
| `_score_etags`                                       | `int`    | ETags score.                                      |
| `_score_gzip`                                        | `int`    | Gzip compression score.                           |
| `_score_keep-alive`                                  | `int`    | Keep-alive score.                                 |
| `_score_minify`                                      | `int`    | Minification score.                               |
| `_securityDetails`                                   | `object` | Security details of the request.                  |
| `_securityDetails.certificateId`                     | `int`    | Certificate ID.                                   |
| `_securityDetails.certificateTransparencyCompliance` | `string` | Certificate transparency compliance.              |
| `_securityDetails.cipher`                            | `string` | Cipher used.                                      |
| `_securityDetails.encryptedClientHello`              | `int`    | Indicates if the client hello is encrypted.       |
| `_securityDetails.issuer`                            | `string` | Issuer of the certificate.                        |
| `_securityDetails.keyExchange`                       | `string` | Key exchange used.                                |
| `_securityDetails.keyExchangeGroup`                  | `string` | Key exchange group used.                          |
| `_securityDetails.protocol`                          | `string` | Security protocol used.                           |
| `_securityDetails.sanList`                           | `array`  | Subject alternative names.                        |
| `_securityDetails.serverSignatureAlgorithm`          | `int`    | Server signature algorithm.                       |
| `_securityDetails.signedCertificateTimestampList`    | `array`  | List of signed certificate timestamps.            |
| `_securityDetails.subjectName`                       | `string` | Subject name of the certificate.                  |
| `_securityDetails.validFrom`                         | `int`    | Valid from date of the certificate.               |
| `_securityDetails.validTo`                           | `int`    | Valid to date of the certificate.                 |
| `_server_count`                                      | `int`    | Number of servers used.                           |
| `_server_port`                                       | `string` | Server port.                                      |
| `_server_rtt`                                        | `int`    | Server round-trip time.                           |
| `_socket_group`                                      | `string` | Socket group.                                     |
| `_socket`                                            | `int`    | Socket used for the request.                      |
| `_ssl_end`                                           | `int`    | SSL handshake end time.                           |
| `_ssl_ms`                                            | `int`    | SSL handshake time in milliseconds.               |
| `_ssl_start`                                         | `int`    | SSL handshake start time.                         |
| `_tls_cipher_suite`                                  | `int`    | Cipher suite used.                                |
| `_tls_next_proto`                                    | `string` | Next protocol used.                               |
| `_tls_resumed`                                       | `string` | Indicates if the TLS session was resumed.         |
| `_tls_version`                                       | `string` | TLS version used.                                 |
| `_ttfb_end`                                          | `int`    | Time to first byte end time.                      |
| `_ttfb_ms`                                           | `int`    | Time to first byte in milliseconds.               |
| `_ttfb_start`                                        | `int`    | Time to first byte start time.                    |
| `_type`                                              | `int`    | Type identifier for the request.                  |
| `_url`                                               | `string` | URL path of the request.                          |
| `cache`                                              | `object` | Cache details (empty in this example).            |
| `pageref`                                            | `string` | Reference to the page containing this request.    |
| `request`                                            | `object` | Details of the request.                           |
| `request.bodySize`                                   | `int`    | Size of the request body.                         |
| `request.cookies`                                    | `array`  | Cookies sent with the request.                    |
| `request.headersSize`                                | `int`    | Size of the request headers.                      |
| `request.httpVersion`                                | `string` | HTTP version used for the request.                |
| `request.method`                                     | `string` | HTTP method used for the request.                 |
| `request.queryString`                                | `array`  | Query string parameters.                          |
| `request.url`                                        | `string` | URL of the requested resource.                    |
| `response`                                           | `object` | Details of the response.                          |
| `response.bodySize`                                  | `int`    | Size of the response body.                        |
| `response.content.mimeType`                          | `string` | MIME type of the content.                         |
| `response.content.size`                              | `int`    | Size of the content.                              |
| `response.content`                                   | `object` | Content details of the response.                  |
| `response.cookies`                                   | `array`  | Cookies received with the response.               |
| `response.headersSize`                               | `int`    | Size of the response headers.                     |
| `response.httpVersion`                               | `string` | HTTP version used for the response.               |
| `response.status`                                    | `int`    | HTTP response status code.                        |
| `response.statusText`                                | `string` | Status text of the response.                      |
| `startedDateTime`                                    | `string` | Start time of the request.                        |
| `time`                                               | `int`    | Total time taken for the request in milliseconds. |
| `timings`                                            | `object` | Timing details of various stages of the request.  |
| `timings.blocked`                                    | `int`    | Time spent in blocking.                           |
| `timings.connect`                                    | `int`    | Time spent in establishing a connection.          |
| `timings.dns`                                        | `int`    | Time spent in DNS lookup.                         |
| `timings.receive`                                    | `int`    | Time spent in receiving the response.             |
| `timings.send`                                       | `int`    | Time spent in sending the request.                |
| `timings.ssl`                                        | `int`    | Time spent in SSL handshake.                      |
| `timings.wait`                                       | `int`    | Time spent in waiting for the response.           |

### `_all_end`

End time of all operations.

### `_all_ms`

Total time taken for all operations.

### `_all_start`

Start time of all operations.

### `_body_file`

File containing the body of the request.

### `_bytesIn`

Number of bytes received.

### `_bytesOut`

Number of bytes sent.

### `_cacheControl`

Cache control header value.

### `_cache_time`

Cache time.

### `_cached`

Indicates if the request was cached (0 or 1).

### `_cdn_provider`

CDN provider used.

### `_certificates`

array | Certificates used.

### `_chunks`

array | Array of chunks received.

- #### `_chunks[].bytes`

  Size of the chunk.

- #### `_chunks[].inflated`

  Size of the inflated chunk.

- #### `_chunks[].ts`

  Timestamp of the chunk.

### `_connect_end`

Connection end time.

### `_connect_ms`

Connection time in milliseconds.

### `_connect_start`

Connection start time.

### `_contentEncoding`

Content encoding of the response.

### `_contentType`

Content type of the response.

### `_created`

Creation time of the request.

### `_dns_end`

DNS end time.

### `_dns_info`

DNS information.

- #### `_dns_info.results`

  Results of the DNS query.

- #### `_dns_info.results.aliases`

  Aliases for the domain.

- #### `_dns_info.results.canonical_names`

  Canonical names for the domain.

- #### `_dns_info.results.endpoint_metadatas`

  Endpoint metadata.

- #### `_dns_info.results.expiration`

  Expiration date of the DNS query.

- #### `_dns_info.results.host_ports`

  Host ports.

- #### `_dns_info.results.hostname_results`

  Hostname results.

- #### `_dns_info.results.ip_endpoints`

  IP endpoints.

- #### `_dns_info.results.ip_endpoints[].endpoint_address`

  IP address of the endpoint.

- #### `_dns_info.results.ip_endpoints[].endpoint_port`

  Port of the endpoint.

- #### `_dns_info.results.text_records`

  Text records.

- #### `_dns_info.secure`

  Indicates if the DNS query is secure.

- #### `_dns_info.transactions_needed`

  Transactions needed for DNS query.

- #### `_dns_info.transactions_needed[].dns_query_type`

  Type of DNS query.

### `_dns_ms`

DNS lookup time in milliseconds.

### `_dns_start`

DNS start time.

### `_documentURL`

Document URL of the request.

### `_download_end`

Download end time.

### `_download_ms`

Download time in milliseconds.

### `_download_start`

Download start time.

### `_expires`

Expiry date of the request.

### `_final_base_page`

Indicates if the request is the final base page.

### `_frame_id`

Frame ID where the request was made.

### `_full_url`

Full URL of the request.

### `_gzip_save`

Size saved due to gzip compression.

### `_gzip_total`

Total size of the gzip-compressed content.

### `_host`

Host of the request.

### `_http2_server_settings`

HTTP/2 server settings.

### `_http2_stream_dependency`

HTTP/2 stream dependency.

### `_http2_stream_exclusive`

HTTP/2 stream exclusivity.

### `_http2_stream_id`

HTTP/2 stream ID.

### `_http2_stream_weight`

HTTP/2 stream weight.

### `_id`

Unique identifier for the request.

### `_image_save`

Size saved due to image optimization.

### `_image_total`

Total size of images.

### `_index`

Index of the request.

### `_initial_priority`

Initial priority of the request.

### `_initiator`

Initiator of the request.

### `_initiator_column`

Column number of the initiator.

### `_initiator_line`

Line number of the initiator.

### `_initiator_type`

Type of initiator (e.g., script).

### `_ip_addr`

IP address of the requested server.

### `_is_base_page`

Indicates if the request is the base page.

### `_is_secure`

Indicates if the request is secure (0 or 1).

### `_load_end`

Load end time.

### `_load_ms`

Load time in milliseconds.

### `_load_start`

Start time of load in milliseconds.

### `_load_start_float`

float | Precise start time of load.

### `_method`

HTTP method used for the request.

### `_minify_save`

Size saved due to minification.

### `_minify_total`

Total size of minified content.

### `_netlog_id`

Netlog ID.

### `_number`

Number of the request.

### `_objectSize`

Size of the object received.

### `_objectSizeUncompressed`

Uncompressed size of the object received.

### `_priority`

Priority of the request.

### `_protocol`

Protocol used for the request.

### `_raw_id`

Raw ID for the request.

### `_request_id`

Identifier for the original request.

### `_request_type`

Type of the request (e.g., Document).

### `_responseCode`

HTTP response code.

### `_run`

The run number of the test.

### `_score_cache`

Cache score.

### `_score_cdn`

CDN score.

### `_score_combine`

Combine score.

### `_score_compress`

Compression score.

### `_score_cookies`

Cookies score.

### `_score_etags`

ETags score.

### `_score_gzip`

Gzip compression score.

### `_score_keep-alive`

Keep-alive score.

### `_score_minify`

Minification score.

### `_securityDetails`

Security details of the request.

- #### `_securityDetails.certificateId`

  Certificate ID.

- #### `_securityDetails.certificateTransparencyCompliance`

  Certificate transparency compliance.

- #### `_securityDetails.cipher`

  Cipher used.

- #### `_securityDetails.encryptedClientHello`

  Indicates if the client hello is encrypted.

- #### `_securityDetails.issuer`

  Issuer of the certificate.

- #### `_securityDetails.keyExchange`

  Key exchange used.

- #### `_securityDetails.keyExchangeGroup`

  Key exchange group used.

- #### `_securityDetails.protocol`

  Security protocol used.

- #### `_securityDetails.sanList`

  Subject alternative names.

- #### `_securityDetails.serverSignatureAlgorithm`

  Server signature algorithm.

- #### `_securityDetails.signedCertificateTimestampList`

  List of signed certificate timestamps.

- #### `_securityDetails.subjectName`

  Subject name of the certificate.

- #### `_securityDetails.validFrom`

  Valid from date of the certificate.

- #### `_securityDetails.validTo`

  Valid to date of the certificate.

### `_server_count`

Number of servers used.

### `_server_port`

Server port.

### `_server_rtt`

Server round-trip time.

### `_socket`

Socket used for the request.

### `_socket_group`

Socket group.

### `_ssl_end`

SSL handshake end time.

### `_ssl_ms`

SSL handshake time in milliseconds.

### `_ssl_start`

SSL handshake start time.

### `_tls_cipher_suite`

Cipher suite used.

### `_tls_next_proto`

Next protocol used.

### `_tls_resumed`

Indicates if the TLS session was resumed.

### `_tls_version`

TLS version used.

### `_ttfb_end`

Time to first byte end time.

### `_ttfb_ms`

Time to first byte in milliseconds.

### `_ttfb_start`

Time to first byte start time.

### `_type`

Type identifier for the request.

### `_url`

URL path of the request.

### `cache`

Cache details (empty in this example).

### `pageref`

Reference to the page containing this request.

### `request`

Details of the request.

- #### `request.bodySize`

  Size of the request body.

- #### `request.cookies`

  Cookies sent with the request.

- #### `request.headersSize`

  Size of the request headers.

- #### `request.httpVersion`

  HTTP version used for the request.

- #### `request.method`

  HTTP method used for the request.

- #### `request.queryString`

  Query string parameters.

- #### `request.url`

  URL of the requested resource.

### `response`

Details of the response.

- #### `response.bodySize`

  Size of the response body.

- #### `response.content`

  Content details of the response.

- #### `response.content.mimeType`

  MIME type of the content.

- #### `response.content.size`

  Size of the content.

- #### `response.cookies`

  Cookies received with the response.

- #### `response.headersSize`

  Size of the response headers.

- #### `response.httpVersion`

  HTTP version used for the response.

- #### `response.status`

  HTTP response status code.

- #### `response.statusText`

  Status text of the response.

### `startedDateTime`

Start time of the request.

### `time`

Total time taken for the request in milliseconds.

### `timings`

Timing details of various stages of the request.

- #### `timings.blocked`

  Time spent in blocking.

- #### `timings.connect`

  Time spent in establishing a connection.

- #### `timings.dns`

  Time spent in DNS lookup.

- #### `timings.receive`

  Time spent in receiving the response.

- #### `timings.send`

  Time spent in sending the request.

- #### `timings.ssl`

  Time spent in SSL handshake.

- #### `timings.wait`

  Time spent in waiting for the response.
