# Errata 6656 - RFC 8588

- **RFC Title:** Personal Assertion Token (PaSSporT) Extension for Signature-based Handling of Asserted information using toKENs (SHAKEN)
- **RFC Publication Date:** May 2019

```
Section 6 says:


Protected Header

   {

      "alg":"ES256",

      "typ":"passport",

      "ppt":"shaken",

      "x5u":"https://cert.example.org/passport.cer"

   }

   Payload

   {

      "attest":"A"

      "dest":{"tn":["12155550131"]}

      "iat":"1443208345",

      "orig":{"tn":"12155550121"},

      "origid":"123e4567-e89b-12d3-a456-426655440000"

   }

// state how to fix the above text here

```

## Issue description

The original example uses a value of an incorrect data type for a property according to RFC 8225.
