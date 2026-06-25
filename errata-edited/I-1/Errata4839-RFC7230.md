# Errata 4839 - RFC 7230

- **RFC Title:** Hypertext Transfer Protocol (HTTP/1.1): Message Syntax and Routing
- **RFC Publication Date:** June 2014

```
Section 4 says:


   Parameters are in the form of a name or name=value pair.



     transfer-parameter = token BWS "=" BWS ( token / quoted-string )

// state how to fix the above text here

```

## Issue description

Section 4 of RFC 7230 contains a contradiction between the prose description of transfer parameters and the corresponding ABNF definition, creating ambiguity about what forms a valid transfer parameter may take.
