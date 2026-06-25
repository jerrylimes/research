# Errata 4949 - RFC 7252

- **RFC Title:** The Constrained Application Protocol (CoAP)
- **RFC Publication Date:** June 2014
```
Section 5.10.7 says:


If any

of these reserved option numbers occurs in addition to Location-Path

and/or Location-Query and are not supported, then a 4.02 (Bad Option)

error MUST be returned.

// state how to fix the above text here

```

## Issue description

The original text in Section 5.10.7 does not handle unsupported reserved option numbers correctly. This inconsistency impacts implementations that rely on the original specification to handle these responses correctly.
