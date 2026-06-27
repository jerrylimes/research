# Errata 4948 - RFC 7252

- **RFC Title:** The Constrained Application Protocol (CoAP)
- **RFC Publication Date:** June 2014

```
Section 5.6 says:


For a presented request, a CoAP endpoint MUST NOT use a stored

response, unless:



o  the presented request method and that used to obtain the stored

   response match,



o  all options match between those in the presented request and those

   of the request used to obtain the stored response (which includes

   the request URI), except that there is no need for a match of any

   request options marked as NoCacheKey (Section 5.4) or recognized

   by the Cache and fully interpreted with respect to its specified

   cache behavior (such as the ETag request option described in

   Section 5.10.6; see also Section 5.4.2), and



o  the stored response is either fresh or successfully validated as

   defined below.



The set of request options that is used for matching the cache entry

is also collectively referred to as the "Cache-Key".

// state how to fix the above text here

```

## Issue description

The original specification for cache key matching does not account for all components of a request that may affect how a server generate its response, leading to inconsistencies in handling cached responses. This inconsistency directly affects cache behavior and may lead to unexpected results in implementations that do not consider the payload when generating the cache key.
