# Errata 4825 - RFC 7230

- **RFC Title:** Hypertext Transfer Protocol (HTTP/1.1): Message Syntax and Routing
- **RFC Publication Date:** June 2014

```
Section Appendix B says:


chunk-ext      = *( ";" chunk-ext-name [ "=" chunk-ext-val ] )

// state how to fix the above text here

Notes:

The infamous "implicit *LWS" syntax rule in RFC 2616 allowed some extent of flexibility in chunk-ext. Moreover, ICAP, which generally relies on HTTP/1 for its message syntax, uses that flexibility when defining the "ieof" chunk extension in RFC 3507 Section 4.5, which is provided below.

Section 4.5:


\r\n

0; ieof\r\n\r\n

```

## Explanation

The erratum highlights an inconsistency between the ABNF rule for `chunk-ext` in Appendix B of RFC 7230 and the actual practices observed in HTTP and ICAP implementations. The original specification does not allow whitespace around semicolons and equals signs within `chunk-ext`, while some HTTP agents generate and parse such whitespace, and RFC 2616 implicitly allowed this.  This inconsistency affects interoperability. The proposed change to include optional whitespace improves compatibility with existing implementations and clarifies the specification, addressing a conflict between the RFC and practical implementations.
