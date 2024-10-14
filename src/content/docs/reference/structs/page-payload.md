---
title: Pages payload struct
description: Reference docs for the page payload struct
---

_Appears in: [`pages` table](/reference/tables/pages/#payload)_\
_As: `payload`_

JSON-encoded WebPageTest result data for a page.

Here's an example of the decoded object:

```json
{
    "_LargestContentfulPaintNodeType": "P",
    "_LargestContentfulPaintType": "text",
    "_LastInteractive": 400,
    "_PerformancePaintTiming.first-contentful-paint": 314.80000000447035,
    "_PerformancePaintTiming.first-paint": 314.80000000447035,
    "_SpeedIndex": 400,
    "_TTFB": 232,
    "_TTIMeasurementEnd": 3452,
    "_URL": "https://www.example.com/",
    "_aft": 0,
    "_audit_issues": [
        {
            "code": "QuirksModeIssue",
            "details": {
                "quirksModeIssueDetails": {
                    "documentNodeId": 2,
                    "frameId": "E021D0149DE3689992ECE4DF4B0ECA38",
                    "isLimitedQuirksMode": false,
                    "loaderId": "67DD39DE1A5C91FCB7B25B32EB8F7231",
                    "url": "http://127.0.0.1:8888/orange.html"
                }
            }
        }
    ],
    "_basePageSSLTime": 98,
    "_base_page_cdn": "Edgecast",
    "_base_page_cname": "",
    "_base_page_dns_server": "a.iana-servers.net",
    "_base_page_ip_ptr": "",
    "_browserVersion": "128.0.0.0",
    "_browser_name": "Chrome",
    "_browser_version": "128.0.0.0",
    "_bytesIn": 1296,
    "_bytesInDoc": 1296,
    "_bytesOut": 4112,
    "_bytesOutDoc": 4112,
    "_cached": 0,
    "_chromeUserTiming": [
        {
            "name": "navigationStart",
            "time": 39
        },
        ...
    ],
    "_chromeUserTiming.CumulativeLayoutShift": 0,
    "_chromeUserTiming.LargestContentfulPaint": 354,
    "_chromeUserTiming.LargestTextPaint": 354,
    "_chromeUserTiming.TotalLayoutShift": 0,
    "_chromeUserTiming.commitNavigationEnd": 285,
    "_chromeUserTiming.domComplete": 320,
    "_chromeUserTiming.domContentLoadedEventEnd": 320,
    "_chromeUserTiming.domContentLoadedEventStart": 320,
    "_chromeUserTiming.domInteractive": 320,
    "_chromeUserTiming.domLoading": 285,
    "_chromeUserTiming.fetchStart": 48,
    "_chromeUserTiming.firstContentfulPaint": 354,
    "_chromeUserTiming.firstMeaningfulPaint": 354,
    "_chromeUserTiming.firstMeaningfulPaintCandidate": 354,
    "_chromeUserTiming.firstPaint": 354,
    "_chromeUserTiming.loadEventEnd": 320,
    "_chromeUserTiming.loadEventStart": 320,
    "_chromeUserTiming.markAsMainFrame": 284,
    "_chromeUserTiming.navigationStart": 74,
    "_chromeUserTiming.responseEnd": 277,
    "_chromeUserTiming.unloadEventEnd": 284,
    "_chromeUserTiming.unloadEventStart": 284,
    "_connections": 1,
    "_consoleLog": [
        {
            "level": "error",
            "networkRequestId": "344808.2",
            "source": "network",
            "text": "Failed to load resource: the server responded with a status of 404 ()",
            "timestamp": 1726370503561.599,
            "url": "https://www.example.com/favicon.ico"
        }
    ],
    "_cpu.CommitLoad": 0,
    "_cpu.EventDispatch": 0,
    "_cpu.FunctionCall": 0,
    "_cpu.HTMLDocumentParser::FetchQueuedPreloads": 0,
    "_cpu.Idle": 302,
    "_cpu.Layerize": 0,
    "_cpu.Layout": 18,
    "_cpu.MarkDOMContent": 0,
    "_cpu.MarkLoad": 0,
    "_cpu.Paint": 0,
    "_cpu.ParseHTML": 2,
    "_cpu.PrePaint": 0,
    "_cpu.ResourceFetcher::requestResource": 0,
    "_cpu.UpdateLayoutTree": 0,
    "_cpu.V8.GC_TIME_TO_SAFEPOINT": 0,
    "_cpu.largestContentfulPaint::Candidate": 0,
    "_cpuTimes": {
        "CommitLoad": 0,
        "EventDispatch": 0,
        "FunctionCall": 0,
        "HTMLDocumentParser::FetchQueuedPreloads": 0,
        "Idle": 302,
        "Layerize": 0,
        "Layout": 18,
        "MarkDOMContent": 0,
        "MarkLoad": 0,
        "Paint": 0,
        "ParseHTML": 2,
        "PrePaint": 0,
        "ResourceFetcher::requestResource": 0,
        "UpdateLayoutTree": 0,
        "V8.GC_TIME_TO_SAFEPOINT": 0,
        "largestContentfulPaint::Candidate": 0
    },
    "_cpuTimesDoc": {
        "CommitLoad": 0,
        "EventDispatch": 0,
        "FunctionCall": 0,
        "HTMLDocumentParser::FetchQueuedPreloads": 0,
        "Idle": 299,
        "Layerize": 0,
        "Layout": 18,
        "MarkDOMContent": 0,
        "MarkLoad": 0,
        "Paint": 0,
        "ParseHTML": 2,
        "PrePaint": 0,
        "ResourceFetcher::requestResource": 0,
        "UpdateLayoutTree": 0,
        "V8.GC_TIME_TO_SAFEPOINT": 0,
        "largestContentfulPaint::Candidate": 0
    },
    "_date": 1726370503.1648238,
    "_docTime": 320,
    "_document_URL": "https://www.example.com/",
    "_document_hostname": "www.example.com",
    "_document_origin": "https://www.example.com",
    "_domComplete": 281,
    "_domContentLoadedEventEnd": 280,
    "_domContentLoadedEventStart": 280,
    "_domElements": 12,
    "_domInteractive": 280,
    "_domLoading": 0,
    "_domTime": 0,
    "_edge-processed": true,
    "_effectiveBps": 14727,
    "_eventName": "Step_1",
    "_execution_contexts": [
        {
            "id": 1,
            "name": "",
            "origin": "https://www.example.com"
        },
        ...
    ],
    "_final_base_page_request": 0,
    "_final_base_page_request_id": "44714C6F6C72B045136D19CA9894886A",
    "_final_url": "https://www.example.com/",
    "_firstContentfulPaint": 354,
    "_firstMeaningfulPaint": 354,
    "_firstPaint": 314.80000000447035,
    "_fullyLoaded": 323,
    "_fullyLoadedCPUms": 610,
    "_fullyLoadedCPUpct": 9.41358024700691,
    "_gzip_savings": 0,
    "_gzip_total": 648,
    "_image_savings": 0,
    "_image_total": 0,
    "_interactivePeriods": [[0, 3452]],
    "_largestPaints": [
        {
            "DOMNodeId": 3,
            "event": "LargestTextPaint",
            "nodeInfo": {
                "bounds": [660, 192.875, 600, 57],
                "nodeType": "P",
                "styles": {
                    "background-image": "none"
                }
            },
            "size": 33858,
            "time": 354
        }
    ],
    "_lastVisualChange": 400,
    "_lighthouse.Accessibility": 0.88,
    "_lighthouse.BestPractices": 0.96,
    "_lighthouse.Performance": 1,
    "_lighthouse.Performance.cumulative-layout-shift": 0,
    "_lighthouse.Performance.first-contentful-paint": 329.542,
    "_lighthouse.Performance.largest-contentful-paint": 329.542,
    "_lighthouse.Performance.speed-index": 322,
    "_lighthouse.Performance.total-blocking-time": 0,
    "_lighthouse.SEO": 0.9,
    "_loadEventEnd": 281,
    "_loadEventStart": 281,
    "_loadTime": 320,
    "_main_frame": "E021D0149DE3689992ECE4DF4B0ECA38",
    "_minify_savings": -1,
    "_minify_total": -1,
    "_optimization_checked": 1,
    "_origin_dns": {
        "cname": [],
        "https": [],
        "mx": ["0 ."],
        "ns": [
            "a.iana-servers.net.",
            "b.iana-servers.net."
        ],
        "soa": [
            "ns.icann.org. noc.dns.icann.org. 2024081420 7200 3600 1209600 3600"
        ],
        "svcb": [],
        "txt": [
            "\"v=spf1 -all\"",
            "\"wgyf8z8cgvm2qmxpnbnldrcltvk4xqfn\""
        ]
    },
    "_osPlatform": "x86_64 x86_64",
    "_osVersion": "Linux 6.8.0-1014-gcp",
    "_os_version": "Linux 6.8.0-1014-gcp",
    "_render": 400,
    "_renderBlockingCSS": 0,
    "_renderBlockingJS": 0,
    "_requests": 2,
    "_requestsDoc": 2,
    "_requestsFull": 2,
    "_responses_200": 1,
    "_responses_404": 1,
    "_responses_other": 0,
    "_result": 99999,
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
    "_score_progressive_jpeg": -1,
    "_server_rtt": 0,
    "_start_epoch": 1726370501.1809506,
    "_step": 1,
    "_testID": "240912_Dx1XE_EVGML",
    "_testStartOffset": 0,
    "_testUrl": "https://www.example.com/",
    "_test_run_time_ms": 5850,
    "_tester": "agents-west-1-kl42-10.138.2.146",
    "_titleTime": 76,
    "_v8Stats": {
        "background": {},
        "main_thread": {}
    },
    "_viewport": {
        "dpr": 1,
        "height": 993,
        "width": 1920
    },
    "_visualComplete": 400,
    "_visualComplete85": 400,
    "_visualComplete90": 400,
    "_visualComplete95": 400,
    "_visualComplete99": 400,
    "id": "page_1_0_1",
    "pageTimings": {
        "_startRender": 400,
        "onContentLoad": -1,
        "onLoad": 320
    },
    "startedDateTime": "2024-09-15T03:21:42.914962",
    "testID": "240912_Dx1XE_EVGML",
    "title": "Run 1, First View for https://www.example.com/"
}
```

## Schema

Field | Type | Description
-- | -- | --
[`_LargestContentfulPaintNodeType`](#_largestcontentfulpaintnodetype) | `string` | The node type of the largest contentful paint
[`_LargestContentfulPaintType`](#_largestcontentfulpainttype) | `string` | The type of the largest contentful paint
[`_LastInteractive`](#_lastinteractive) | `int` | The time when the page was last interactive in milliseconds
[`_PerformancePaintTiming.first-contentful-paint`](#_performancepainttimingfirst-contentful-paint) | `float` | The time when the first contentful paint occurred in milliseconds
[`_PerformancePaintTiming.first-paint`](#_performancepainttimingfirst-paint) | `float` | The time when the first paint occurred in milliseconds
[`_SpeedIndex`](#_speedindex) | `int` | The Speed Index score
[`_TTFB`](#_ttfb) | `int` | The time to first byte in milliseconds
[`_TTIMeasurementEnd`](#_ttimeasurementend) | `int` | The time when the TTI measurement ended in milliseconds
[`_URL`](#_url) | `string` | The URL of the page
[`_aft`](#_aft) | `int` | The above-the-fold time in milliseconds
[`_audit_issues`](#_audit_issues) | `array` | Audit issues
[`_basePageSSLTime`](#_basepagessltime) | `int` | The time spent on SSL for the base page in milliseconds
[`_base_page_cdn`](#_base_page_cdn) | `string` | The CDN used for the base page
[`_base_page_cname`](#_base_page_cname) | `string` | The CNAME used for the base page
[`_base_page_dns_server`](#_base_page_dns_server) | `string` | The DNS server used for the base page
[`_base_page_ip_ptr`](#_base_page_ip_ptr) | `string` | The IP PTR used for the base page
[`_browserVersion`](#_browserversion) | `string` | The browser version
[`_browser_name`](#_browser_name) | `string` | The browser name
[`_browser_version`](#_browser_version) | `string` | The browser version
[`_bytesIn`](#_bytesin) | `int` | The number of bytes received in
[`_bytesInDoc`](#_bytesindoc) | `int` | The number of bytes received in the document
[`_bytesOut`](#_bytesout) | `int` | The number of bytes sent out
[`_bytesOutDoc`](#_bytesoutdoc) | `int` | The number of bytes sent out in the
[`_cached`](#_cached) | `int` | Whether the page was cached
[`_chromeUserTiming`](#_chromeusertiming) | `array` | Chrome user timing
[`_chromeUserTiming.CumulativeLayoutShift`](#_chromeusertimingcumulativelayoutshift) | `int` | The cumulative layout shift
[`_chromeUserTiming.LargestContentfulPaint`](#_chromeusertiminglargestcontentfulpaint) | `int` | The largest contentful paint
[`_chromeUserTiming.LargestTextPaint`](#_chromeusertiminglargesttextpaint) | `int` | The largest text paint
[`_chromeUserTiming.TotalLayoutShift`](#_chromeusertimingtotallayoutshift) | `int` | The total layout shift
[`_chromeUserTiming.commitNavigationEnd`](#_chromeusertimingcommitnavigationend) | `int` | The commit navigation end
[`_chromeUserTiming.domComplete`](#_chromeusertimingdomcomplete) | `int` | The DOM complete
[`_chromeUserTiming.domContentLoadedEventEnd`](#_chromeusertimingdomcontentloadedeventend) | `int` | The DOM content loaded event end
[`_chromeUserTiming.domContentLoadedEventStart`](#_chromeusertimingdomcontentloadedeventstart) | `int` | The DOM content loaded event start
[`_chromeUserTiming.domInteractive`](#_chromeusertimingdominteractive) | `int` | The DOM interactive
[`_chromeUserTiming.domLoading`](#_chromeusertimingdomloading) | `int` | The DOM loading
[`_chromeUserTiming.fetchStart`](#_chromeusertimingfetchstart) | `int` | The fetch start
[`_chromeUserTiming.firstContentfulPaint`](#_chromeusertimingfirstcontentfulpaint) | `int` | The first contentful paint
[`_chromeUserTiming.firstMeaningfulPaint`](#_chromeusertimingfirstmeaningfulpaint) | `int` | The first meaningful paint
[`_chromeUserTiming.firstMeaningfulPaintCandidate`](#_chromeusertimingfirstmeaningfulpaintcandidate) | `int` | The first meaningful paint candidate
[`_chromeUserTiming.firstPaint`](#_chromeusertimingfirstpaint) | `int` | The first paint
[`_chromeUserTiming.loadEventEnd`](#_chromeusertimingloadeventend) | `int` | The load event end
[`_chromeUserTiming.loadEventStart`](#_chromeusertimingloadeventstart) | `int` | The load event start
[`_chromeUserTiming.markAsMainFrame`](#_chromeusertimingmarkasmainframe) | `int` | The mark as main frame
[`_chromeUserTiming.navigationStart`](#_chromeusertimingnavigationstart) | `int` | The navigation start
[`_chromeUserTiming.responseEnd`](#_chromeusertimingresponseend) | `int` | The response end
[`_chromeUserTiming.unloadEventEnd`](#_chromeusertimingunloadeventend) | `int` | The unload event end
[`_chromeUserTiming.unloadEventStart`](#_chromeusertimingunloadeventstart) | `int` | The unload event start
[`_connections`](#_connections) | `int` | The number of connections
[`_consoleLog`](#_consolelog) | `array` | Console logs
[`_cpu.CommitLoad`](#_cpucommitload) | `int` | The CPU time spent on commit load in milliseconds
[`_cpu.EventDispatch`](#_cpueventdispatch) | `int` | The CPU time spent on event dispatch in milliseconds
[`_cpu.FunctionCall`](#_cpufunctioncall) | `int` | The CPU time spent on function call in milliseconds
[`_cpu.HTMLDocumentParser::FetchQueuedPreloads`](#_cpuhtmldocumentparserfetchqueuedpreloads) | `int` | The CPU time spent on HTML document parser fetch queued preloads in milliseconds
[`_cpu.Idle`](#_cpuidle) | `int` | The CPU time spent on idle in milliseconds
[`_cpu.Layerize`](#_cpulayerize) | `int` | The CPU time spent on layerize in milliseconds
[`_cpu.Layout`](#_cpulayout) | `int` | The CPU time spent on layout in milliseconds
[`_cpu.MarkDOMContent`](#_cpumarkdomcontent) | `int` | The CPU time spent on marking DOM content in milliseconds
[`_cpu.MarkLoad`](#_cpumarkload) | `int` | The CPU time spent on marking load in milliseconds
[`_cpu.Paint`](#_cpupaint) | `int` | The CPU time spent on paint in milliseconds
[`_cpu.ParseHTML`](#_cpuparsehtml) | `int` | The CPU time spent on parsing HTML in milliseconds
[`_cpu.PrePaint`](#_cpuprepaint) | `int` | The CPU time spent on pre-paint in milliseconds
[`_cpu.ResourceFetcher::requestResource`](#_cpuresourcefetcherrequestresource) | `int` | The CPU time spent on resource fetcher request resource in milliseconds
[`_cpu.UpdateLayoutTree`](#_cpuupdatelayouttree) | `int` | The CPU time spent on updating layout tree in milliseconds
[`_cpu.V8.GC_TIME_TO_SAFEPOINT`](#_cpuv8gc_timeto_safepoint) | `int` | The CPU time spent on V8 GC time to safepoint in milliseconds
[`_cpu.largestContentfulPaint::Candidate`](#_cpulargestcontentfulpaintcandidate) | `int` | The CPU time spent on largest contentful paint candidate in milliseconds
[`_cpuTimes`](#_cputimes) | `object` | CPU times
[`_cpuTimesDoc`](#_cputimesdoc) | `object` | CPU times for the document
[`_date`](#_date) | `float` | The date in Unix timestamp format
[`_docTime`](#_doctime) | `int` | The document time in milliseconds
[`_document_URL`](#_document_url) | `string` | The URL of the document
[`_document_hostname`](#_document_hostname) | `string` | The hostname of the document
[`_document_origin`](#_document_origin) | `string` | The origin of the document
[`_domComplete`](#_domcomplete) | `int` | The DOM complete in milliseconds
[`_domContentLoadedEventEnd`](#_domcontentloadedeventend) | `int` | The DOM content loaded event end in milliseconds
[`_domContentLoadedEventStart`](#_domcontentloadedeventstart) | `int` | The DOM content loaded event start in milliseconds
[`_domElements`](#_domelements) | `int` | The number of DOM elements
[`_domInteractive`](#_dominteractive) | `int` | The DOM interactive in milliseconds
[`_domLoading`](#_domloading) | `int` | The DOM loading in milliseconds
[`_domTime`](#_domtime) | `int` | The DOM time in milliseconds
[`_edge-processed`](#_edge-processed) | `boolean` | Whether the page was processed by Edge
[`_effectiveBps`](#_effectivebps) | `int` | The effective BPS
[`_eventName`](#_eventname) | `string` | The event name
[`_execution_contexts`](#_execution_contexts) | `array` | Execution contexts
[`_final_base_page_request`](#_final_base_page_request) | `int` | The final base page request
[`_final_base_page_request_id`](#_final_base_page_request_id) | `string` | The final base page request ID
[`_final_url`](#_final_url) | `string` | The final URL
[`_firstContentfulPaint`](#_firstcontentfulpaint) | `int` | The first contentful paint in milliseconds
[`_firstMeaningfulPaint`](#_firstmeaningfulpaint) | `int` | The first meaningful paint in milliseconds
[`_firstPaint`](#_firstpaint) | `float` | The first paint in milliseconds
[`_fullyLoaded`](#_fullyloaded) | `int` | The fully loaded time in milliseconds
[`_fullyLoadedCPUms`](#_fullyloadedcpums) | `int` | The fully loaded CPU time in milliseconds
[`_fullyLoadedCPUpct`](#_fullyloadedcpupct) | `float` | The fully loaded CPU percentage
[`_gzip_savings`](#_gzip_savings) | `int` | The bytes saved by gzip compression
[`_gzip_total`](#_gzip_total) | `int` | The total bytes in gzip compression
[`_image_savings`](#_image_savings) | `int` | The bytes saved by image compression
[`_image_total`](#_image_total) | `int` | The total bytes in image compression
[`_interactivePeriods`](#_interactiveperiods) | `array` | Interactive periods
[`_largestPaints`](#_largestpaints) | `array` | Largest paints
[`_lastVisualChange`](#_lastvisualchange) | `int` | The time of the last visual change in milliseconds
[`_lighthouse.Accessibility`](#_lighthouseaccessibility) | `float` | The Lighthouse accessibility score
[`_lighthouse.BestPractices`](#_lighthousebestpractices) | `float` | The Lighthouse best practices score
[`_lighthouse.Performance`](#_lighthouseperformance) | `float` | The Lighthouse performance score
[`_lighthouse.Performance.cumulative-layout-shift`](#_lighthouseperformancecumulative-layout-shift) | `int` | The Lighthouse cumulative layout shift
[`_lighthouse.Performance.first-contentful-paint`](#_lighthouseperformancefirst-contentful-paint) | `float` | The Lighthouse first contentful paint
[`_lighthouse.Performance.largest-contentful-paint`](#_lighthouseperformancelargest-contentful-paint) | `float` | The Lighthouse largest contentful paint
[`_lighthouse.Performance.speed-index`](#_lighthouseperformancespeed-index) | `int` | The Lighthouse speed index
[`_lighthouse.Performance.total-blocking-time`](#_lighthouseperformancetotal-blocking-time) | `int` | The Lighthouse total blocking time
[`_lighthouse.SEO`](#_lighthouseseo) | `float` | The Lighthouse SEO score
[`_loadEventEnd`](#_loadeventend) | `int` | The load event end in milliseconds
[`_loadEventStart`](#_loadeventstart) | `int` | The load event start in milliseconds
[`_loadTime`](#_loadtime) | `int` | The load time in milliseconds
[`_main_frame`](#_main_frame) | `string` | The main frame
[`_minify_savings`](#_minify_savings) | `int` | The bytes saved by minification
[`_minify_total`](#_minify_total) | `int` | The total bytes in minification
[`_optimization_checked`](#_optimization_checked) | `int` | Whether optimization checks were performed
[`_origin_dns`](#_origin_dns) | `object` | Origin DNS
[`_osPlatform`](#_osplatform) | `string` | The OS platform
[`_osVersion`](#_osversion) | `string` | The OS version
[`_os_version`](#_os_version) | `string` | The OS version
[`_render`](#_render) | `int` | The render time in milliseconds
[`_renderBlockingCSS`](#_renderblockingcss) | `int` | The render blocking CSS time in milliseconds
[`_renderBlockingJS`](#_renderblockingjs) | `int` | The render blocking JS time in milliseconds
[`_requests`](#_requests) | `int` | The number of requests
[`_requestsDoc`](#_requestsdoc) | `int` | The number of requests in the document
[`_requestsFull`](#_requestsfull) | `int` | The number of full requests
[`_responses_200`](#_responses_200) | `int` | The number of 200 responses
[`_responses_404`](#_responses_404) | `int` | The number of 404 responses
[`_responses_other`](#_responses_other) | `int` | The number of other responses
[`_result`](#_result) | `int` | The result
[`_run`](#_run) | `int` | The run
[`_score_cache`](#_score_cache) | `int` | The cache score
[`_score_cdn`](#_score_cdn) | `int` | The CDN score
[`_score_combine`](#_score_combine) | `int` | The combine score
[`_score_compress`](#_score_compress) | `int` | The compress score
[`_score_cookies`](#_score_cookies) | `int` | The cookies score
[`_score_etags`](#_score_etags) | `int` | The etags score
[`_score_gzip`](#_score_gzip) | `int` | The gzip score
[`_score_keep-alive`](#_score_keep-alive) | `int` | The keep-alive score
[`_score_minify`](#_score_minify) | `int` | The minify score
[`_score_progressive_jpeg`](#_score_progressive_jpeg) | `int` | The progressive JPEG score
[`_server_rtt`](#_server_rtt) | `int` | The server RTT
[`_start_epoch`](#_start_epoch) | `float` | The start epoch in Unix timestamp format
[`_step`](#_step) | `int` | The step
[`_testID`](#_testid) | `string` | The test ID
[`_testStartOffset`](#_teststartoffset) | `int` | The test start offset
[`_testUrl`](#_testurl) | `string` | The test URL
[`_test_run_time_ms`](#_test_run_time_ms) | `int` | The test run time in milliseconds
[`_tester`](#_tester) | `string` | The tester
[`_titleTime`](#_titletime) | `int` | The title time in milliseconds
[`_v8Stats`](#_v8stats) | `object` | V8 stats
[`_viewport`](#_viewport) | `object` | The viewport
[`_visualComplete`](#_visualcomplete) | `int` | The visual complete time in milliseconds
[`_visualComplete85`](#_visualcomplete85) | `int` | The 85th percentile visual complete time in milliseconds
[`_visualComplete90`](#_visualcomplete90) | `int` | The 90th percentile visual complete time in milliseconds
[`_visualComplete95`](#_visualcomplete95) | `int` | The 95th percentile visual complete time in milliseconds
[`_visualComplete99`](#_visualcomplete99) | `int` | The 99th percentile visual complete time in milliseconds
[`id`](#id) | `string` | The page ID
[`pageTimings`](#pagetimings) | `object` | Page timings
[`startedDateTime`](#starteddatetime) | `string` | The start date and time of the page in Unix timestamp format
[`testID`](#testid) | `string` | The test ID
[`title`](#title) | `string` | The page title

### `_LargestContentfulPaintNodeType`

The node type of the largest contentful paint

### `_LargestContentfulPaintType`

The type of the largest contentful paint

### `_LastInteractive`

The time when the page was last interactive in milliseconds

### `_PerformancePaintTimingfirst-contentful-paint`

The time when the first contentful paint occurred in milliseconds

### `_PerformancePaintTimingfirst-paint`

The time when the first paint occurred in milliseconds

### `_SpeedIndex`

The Speed Index score

### `_TTFB`

The time to first byte in milliseconds

### `_TTIMeasurementEnd`

The time when the TTI measurement ended in milliseconds

### `_URL`

The URL of the page

### `_aft`

The above-the-fold time in milliseconds

### `_audit_issues`

Audit issues

### `_basePageSSLTime`

The time spent on SSL for the base page in milliseconds

### `_base_page_cdn`

The CDN used for the base page

### `_base_page_cname`

The CNAME used for the base page

### `_base_page_dns_server`

The DNS server used for the base page

### `_base_page_ip_ptr`

The IP PTR used for the base page

### `_browserVersion`

The browser version

### `_browser_name`

The browser name

### `_browser_version`

The browser version

### `_bytesIn`

The number of bytes received in

### `_bytesInDoc`

The number of bytes received in the document

### `_bytesOut`

The number of bytes sent out

### `_bytesOutDoc`

The number of bytes sent out in the document

### `_cached`

Whether the page was cached

### `_chromeUserTiming`

Chrome user timing

### `_chromeUserTimingCumulativeLayoutShift`

The cumulative layout shift

### `_chromeUserTimingLargestContentfulPaint`

The largest contentful paint

### `_chromeUserTimingLargestTextPaint`

The largest text paint

### `_chromeUserTimingTotalLayoutShift`

The total layout shift

### `_chromeUserTimingcommitNavigationEnd`

The commit navigation end

### `_chromeUserTimingdomComplete`

The DOM complete

### `_chromeUserTimingdomContentLoadedEventEnd`

The DOM content loaded event end

### `_chromeUserTimingdomContentLoadedEventStart`

The DOM content loaded event start

### `_chromeUserTimingdomInteractive`

The DOM interactive

### `_chromeUserTimingdomLoading`

The DOM loading in milliseconds

### `_chromeUserTimingfetchStart`

The fetch start in milliseconds

### `_chromeUserTimingfirstContentfulPaint`

The first contentful paint

### `_chromeUserTimingfirstMeaningfulPaint`

The first meaningful paint

### `_chromeUserTimingfirstMeaningfulPaintCandidate`

The first meaningful paint candidate

### `_chromeUserTimingfirstPaint`

The first paint

### `_chromeUserTimingloadEventEnd`

The load event end

### `_chromeUserTimingloadEventStart`

The load event start

### `_chromeUserTimingmarkAsMainFrame`

The mark as main frame

### `_chromeUserTimingnavigationStart`

The navigation start

### `_chromeUserTimingresponseEnd`

The response end

### `_chromeUserTimingunloadEventEnd`

The unload event end

### `_chromeUserTimingunloadEventStart`

The unload event start

### `_connections`

The number of connections

### `_consoleLog`

Console logs

### `_cpuCommitLoad`

The CPU time spent on commit load in milliseconds

### `_cpuEventDispatch`

The CPU time spent on event dispatch in milliseconds

### `_cpuFunctionCall`

The CPU time spent on function call in milliseconds

### `_cpuHTMLDocumentParserFetchQueuedPreloads`

The CPU time spent on HTML document parser fetch queued preloads in milliseconds

### `_cpuIdle`

The CPU time spent on idle in milliseconds

### `_cpuLayerize`

The CPU time spent on layerize in milliseconds

### `_cpuLayout`

The CPU time spent on layout in milliseconds

### `_cpuMarkDOMContent`

The CPU time spent on marking DOM content in milliseconds

### `_cpuMarkLoad`

The CPU time spent on marking load in milliseconds

### `_cpuPaint`

The CPU time spent on paint in milliseconds

### `_cpuParseHTML`

The CPU time spent on parsing HTML in milliseconds

### `_cpuPrePaint`

The CPU time spent on pre-paint in milliseconds

### `_cpuResourceFetcherrequestResource`

The CPU time spent on resource fetcher request resource in milliseconds

### `_cpuUpdateLayoutTree`

The CPU time spent on updating layout tree in milliseconds

### `_cpuV8GC_TIMETO_SAFEPOINT`

The CPU time spent on V8 GC time to safepoint in milliseconds

### `_cpulargestContentfulPaintCandidate`

The CPU time spent on largest contentful paint candidate in milliseconds

### `_cpuTimes`

CPU times

### `_cpuTimesDoc`

CPU times for the document

### `_date`

The date in Unix timestamp format

### `_docTime`

The document time in milliseconds

### `_document_URL`

The URL of the document

### `_document_hostname`

The hostname of the document

### `_document_origin`

The origin of the document

### `_domComplete`

The DOM complete in milliseconds

### `_domContentLoadedEventEnd`

The DOM content loaded event end in milliseconds

### `_domContentLoadedEventStart`

The DOM content loaded event start in milliseconds

### `_domElements`

The number of DOM elements

### `_domInteractive`

The DOM interactive in milliseconds

### `_domLoading`

The DOM loading in milliseconds

### `_domTime`

The DOM time in milliseconds

### `_edge-processed`

Whether the page was processed by Edge

### `_effectiveBps`

The effective BPS

### `_eventName`

The event name

### `_execution_contexts`

Execution contexts

### `_final_base_page_request`

The final base page request

### `_final_base_page_request_id`

The final base page request ID

### `_final_url`

The final URL

### `_firstContentfulPaint`

The first contentful paint in milliseconds

### `_firstMeaningfulPaint`

The first meaningful paint in milliseconds

### `_firstPaint`

The first paint in milliseconds

### `_fullyLoaded`

The fully loaded time in milliseconds

### `_fullyLoadedCPUms`

The fully loaded CPU time in milliseconds

### `_fullyLoadedCPUpct`

The fully loaded CPU percentage

### `_gzip_savings`

The bytes saved by gzip compression

### `_gzip_total`

The total bytes in gzip compression

### `_image_savings`

The bytes saved by image compression

### `_image_total`

The total bytes in image compression

### `_interactivePeriods`

Interactive periods in milliseconds

### `_largestPaints`

Largest paints

### `_lastVisualChange`

The time of the last visual change in milliseconds

### `_lighthouseAccessibility`

The Lighthouse accessibility score

### `_lighthouseBestPractices`

The Lighthouse best practices score

### `_lighthousePerformance`

The Lighthouse performance score

### `_lighthousePerformancecumulative-layout-shift`

The Lighthouse cumulative layout shift

### `_lighthousePerformancefirst-contentful-paint`

The Lighthouse first contentful paint

### `_lighthousePerformancelargest-contentful-paint`

The Lighthouse largest contentful paint

### `_lighthousePerformancespeed-index`

The Lighthouse speed index

### `_lighthousePerformancetotal-blocking-time`

The Lighthouse total blocking time

### `_lighthouseSEO`

The Lighthouse SEO score

### `_loadEventEnd`

The load event end in milliseconds

### `_loadEventStart`

The load event start in milliseconds

### `_loadTime`

The load time in milliseconds

### `_main_frame`

The main frame

### `_minify_savings`

The bytes saved by minification

### `_minify_total`

The total bytes in minification

### `_optimization_checked`

Whether optimization checks were performed

### `_origin_dns`

Origin DNS

### `_osPlatform`

The OS platform

### `_osVersion`

The OS version

### `_os_version`

The OS version

### `_render`

The render time in milliseconds

### `_renderBlockingCSS`

The render blocking CSS time in milliseconds

### `_renderBlockingJS`

The render blocking JS time in milliseconds

### `_requests`

The number of requests

### `_requestsDoc`

The number of requests in the document

### `_requestsFull`

The number of full requests

### `_responses_200`

The number of 200 responses

### `_responses_404`

The number of 404 responses

### `_responses_other`

The number of other responses

### `_result`

The result code of the test run

### `_run`

The run number

### `_score_cache`

The cache score

### `_score_cdn`

The CDN score

### `_score_combine`

The combine score

### `_score_compress`

The compress score

### `_score_cookies`

The cookies score

### `_score_etags`

The etags score

### `_score_gzip`

The gzip score

### `_score_keep-alive`

The keep-alive score

### `_score_minify`

The minify score

### `_score_progressive_jpeg`

The progressive JPEG score

### `_server_rtt`

The server RTT

### `_start_epoch`

The start epoch in Unix timestamp format

### `_step`

The step number

### `_testID`

The test ID

### `_testStartOffset`

The test start offset

### `_testUrl`

The test URL

### `_test_run_time_ms`

The test run time in milliseconds

### `_tester`

The tester

### `_titleTime`

The title time in milliseconds

### `_v8Stats`

V8 stats

### `_viewport`

The viewport dimensions

### `_visualComplete`

The visual complete time in milliseconds

### `_visualComplete85`

The 85th percentile visual complete time in milliseconds

### `_visualComplete90`

The 90th percentile visual complete time in milliseconds

### `_visualComplete95`

The 95th percentile visual complete time in milliseconds

### `_visualComplete99`

The 99th percentile visual complete time in milliseconds

### `id`

The page ID

### `pageTimings`

Page timings

### `startedDateTime`

The start date and time of the page in Unix timestamp format

### `testID`

The test ID

### `title`

The page title
