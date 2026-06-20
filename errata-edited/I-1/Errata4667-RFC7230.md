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

The `chunk-ext` ABNF rule in Section 4.1.1 of RFC 7230 does not accommodate whitespace handling that was permitted under RFC 2616 and is widely used in practice, including by ICAP implementations. This creates interoperability issues where HTTP agents may generate messages that strict RFC 7230 parsers cannot handle.
