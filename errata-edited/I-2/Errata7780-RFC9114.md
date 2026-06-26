# Errata 7780 - RFC 9114

- **RFC Title:** HTTP/3
- **RFC Publication Date:** June 2022
- Link to original errata report: [rfc-editor.org/errata/eid7780](https://www.rfc-editor.org/errata/eid7780)

```
Section 7.2.6 says:


The GOAWAY frame applies to the entire connection,

not a specific stream. A client MUST treat a

GOAWAY frame on a stream other than the control

stream as a connection error of type

H3_FRAME_UNEXPECTED.

// state how to fix the above text here

```

## Issue description

The original specification in Section 7.2.6 does not correctly state who must treat the certain type of GOAWAY frame as a connection error. This inconsistency affects the implementation of both clients and servers that must correctly handle GOAWAY frames on streams other than the control stream.
