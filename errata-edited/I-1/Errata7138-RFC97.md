# Errata 7138 - RFC 97

- **RFC Title:** HTTP Semantics
- **RFC Publication Date:** June 2022
- Link to original errata report: [rfc-editor.org/errata/eid7138](https://www.rfc-editor.org/errata/eid7138)

```
Section 12.5.1 says:


The media type quality factor associated with a given type is 

determined by finding the media range with the highest precedence 

that matches the type. For example,



Accept: text/*;q=0.3, text/plain;q=0.7, text/plain;format=flowed,

       text/plain;format=fixed;q=0.4, */*;q=0.5



would cause the following values to be associated:



Table 5: 



Media Type	                Quality Value

text/plain;format=flowed	      1

text/plain	                     0.7

text/html	                     0.3

image/jpeg	                     0.5

text/plain;format=fixed	             0.4

text/html;level=3	             0.7

// state how to fix the above text here

```

## Issue description

The example in Section 12.5.1 contains an incorrect quality value for a media type that cannot be derived from the given Accept header using the precedence rules described in the RFC. This inconsistency between the example and the described algorithm makes the specification unclear and impacts its correct implementation.
