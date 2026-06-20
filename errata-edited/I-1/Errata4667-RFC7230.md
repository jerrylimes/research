# Errata 4667 - RFC 7230

- **RFC Title:** Hypertext Transfer Protocol (HTTP/1.1): Message Syntax and Routing
- **RFC Publication Date:** June 2014
- Link to original errata report: [rfc-editor.org/errata/eid4667](https://www.rfc-editor.org/errata/eid4667)

```
Section 4.1.1 says:


chunk-ext      = *( ";" chunk-ext-name [ "=" chunk-ext-val ] )

// state how to fix the above text here

```

## Issue description

The erratum points to an inconsistency between RFC 7230's definition of `chunk-ext` and the actual practices and implementations observed in HTTP agents and ICAP. This inconsistency creates interoperability issues because HTTP agents might generate whitespace in a way that RFC 7230 does not permit, while parsers adhering strictly to RFC 7230 might fail to parse valid HTTP messages. The proposed correction improves consistency and interoperability with older systems.
