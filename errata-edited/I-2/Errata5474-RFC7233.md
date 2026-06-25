# Errata 5474 - RFC 7233

- **RFC Title:** Hypertext Transfer Protocol (HTTP/1.1): Range Requests
- **RFC Publication Date:** June 2014

```
Section 4.4. says:


For byte ranges, failing to overlap the current extent means that the

   first-byte-pos of all of the byte-range-spec values were greater than

   the current length of the selected representation.

// state how to fix the above text here

```

## Issue description

The description of byte range overlap in Section 4.4 does not fully describe all the possibilities that could lead to failure to overlap the current extent. This error directly impacts the implementation of range request handling, potentially causing servers to incorrectly accept or reject valid or invalid ranges.
