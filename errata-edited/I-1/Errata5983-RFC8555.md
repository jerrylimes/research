# Errata 5983 - RFC 8555

- **RFC Title:** Automatic Certificate Management Environment (ACME)
- **RFC Publication Date:** March 2019
- Link to original errata report: [rfc-editor.org/errata/eid5983](https://www.rfc-editor.org/errata/eid5983)

```
Section 9.1 says:


   A file of this type contains one or more certificates encoded with

   the PEM textual encoding, according to [RFC7468].  The textual

   encoding of certificates in this file MUST use the strict encoding

   and MUST NOT include explanatory text.  The ABNF for this format is

   as follows, where "stricttextualmsg" and "eol" are as defined in

   Section 3 of RFC 7468:



   certchain = stricttextualmsg *(eol stricttextualmsg)

// state how to fix the above text here

```

## Issue description

The ABNF in Section 9.1 is inconsistent with the examples provided in the RFC and the definition of `stricttextualmsg` in RFC 7468. This inconsistency affects the correct interpretation and implementation of the certificate chain format and is therefore classified as INCONSISTENT.
