# Errata 5131 - RFC 8072

- **RFC Title:** YANG Patch Media Type
- **RFC Publication Date:** February 2017

```
Section 2.2 says:


Regarding section 2.2 of RFC 8072, the third paragraph states:





                                       ... If the edit does not identify

    any existing resource instance and the operation for the edit is not

    "create", then the request MUST NOT be processed and a "404 Not

    Found" error response MUST be sent by the server.

// state how to fix the above text here

Notes:

As per the second paragraph of section 2.2 of RFC 8072, the operations are expected to mirror the semantics of the "operation" attribute described in Section 7.2 of [RFC6241].

```

## Issue description

The original specification does not accurately mirror the semantics of the "operation" attribute described in Section 7.2 of RFC6241 like other parts of the Section 2.2 do.
