# Errata 4508 - RFC 7468

- **RFC Title:** Textual Encodings of PKIX, PKCS, and CMS Structures
- **RFC Publication Date:** April 2015

```
Section 3 says:


  preeb      = "-----BEGIN " label "-----" ; unlike [RFC1421] (A)BNF,

                                           ; eol is not required (but

  posteb     = "-----END " label "-----"   ; see [RFC1421], Section 4.4)

// state how to fix the above text here

```

## Issue description

The original ABNF for preeb and posteb does not correctly enforce the case sensitivity of the BEGIN and END keywords. The original ABNF is inconsistent with the actual behavior of implementations and the case sensitivity requirements of the specified encoding.
