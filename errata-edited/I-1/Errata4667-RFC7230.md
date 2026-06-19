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

## Explanation

The erratum points to an inconsistency between RFC 7230's definition of `chunk-ext` and the actual practices and implementations observed in HTTP agents and ICAP. This inconsistency creates interoperability issues because HTTP agents might generate whitespace in a way that RFC 7230 does not permit, while parsers adhering strictly to RFC 7230 might fail to parse valid HTTP messages. The proposed correction improves consistency and interoperability with older systems.
