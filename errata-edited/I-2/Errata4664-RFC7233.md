# Errata 4664 - RFC 7233

- **RFC Title:** Hypertext Transfer Protocol (HTTP/1.1): Range Requests
- **RFC Publication Date:** June 2014

```
Section 4.4 says:


The 416 (Range Not Satisfiable) status code indicates that none of

the ranges in the request's Range header field (Section 3.1) overlap

the current extent of the selected resource or that the set of ranges

requested has been rejected due to invalid ranges or an excessive

request of small or overlapping ranges.

// state how to fix the above text here

```

## Issue description

Section 4.4 does not comprehensively describe what the overlap depends on when there's a 416 status code. The inconsistency affects how servers implement the 416 response, potentially causing incorrect responses in cases where multiple representations exist for the same resource.
