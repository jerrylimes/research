# Errata 6499 - RFC 8224

- **RFC Title:** Authenticated Identity Management in the Session Initiation Protocol (SIP)
- **RFC Publication Date:** February 2018

```
Section 4 says:


Identity = "Identity" HCOLON signed-identity-digest SEMI

          ident-info *( SEMI ident-info-params )

signed-identity-digest = 1*(base64-char / ".")

ident-info = "info" EQUAL ident-info-uri

ident-info-uri = LAQUOT absoluteURI RAQUOT

ident-info-params = ident-info-alg / ident-type /

    ident-info-extension

ident-info-alg = "alg" EQUAL token

ident-type = "ppt" EQUAL token

ident-info-extension = generic-param



base64-char = ALPHA / DIGIT / "/" / "+"

// state how to fix the above text here

```

## Issue description

The original ABNF uses an incorrect encoding that is inconsistent with RFC 8225 and the correct encoding for the signed-identity-digest.
