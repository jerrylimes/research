# Errata 4667 - RFC 7230

- **RFC Title:** Hypertext Transfer Protocol (HTTP/1.1): Message Syntax and Routing
- **RFC Publication Date:** June 2014
- Link to original errata report: [rfc-editor.org/errata/eid4667](https://www.rfc-editor.org/errata/eid4667)

```
Section 4.1.1 says:


chunk-ext      = *( ";" chunk-ext-name [ "=" chunk-ext-val ] )



It should say:

chunk-ext      = *( BWS  ";" BWS chunk-ext-name

                    [ BWS  "=" BWS chunk-ext-val ] )

// state how to fix the above text here

Notes:

The infamous "implicit *LWS" syntax rule in RFC 2616 allowed some extent of flexibility in chunk-ext. Moreover, ICAP, which generally relies on HTTP/1 for its message syntax, uses that flexibility when defining the "ieof" chunk extension in RFC 3507 Section 4.5, which is provided below.

Section 4.5:


\r\n

0; ieof\r\n\r\n


```

## Issue description

The `chunk-ext` ABNF rule in Section 4.1.1 of RFC 7230 does not accommodate whitespace handling that was permitted under RFC 2616 and is widely used in practice, including by ICAP implementations. This creates interoperability issues where HTTP agents may generate messages that strict RFC 7230 parsers cannot handle.
