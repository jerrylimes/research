# Errata 5566 - RFC 8040

- **RFC Title:** RESTCONF Protocol
- **RFC Publication Date:** January 2017

```
Section B.3.2 says:


          "player" : {

            "gap" : 0.5

          }

// state how to fix the above text here

```

## Issue description

The example in Section B.3.2 contradicts RFC 7951, section 6.1, that specifies the correct representation of decimal64 values. This inconsistency affects the correct implementation of JSON serialization for decimal64 types.
