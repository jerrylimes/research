# Errata 6646 - RFC 8366

- **RFC Title:** A Voucher Artifact for Bootstrapping Protocols
- **RFC Publication Date:** May 2018
- Link to original errata report: [rfc-editor.org/errata/eid6646](https://www.rfc-editor.org/errata/eid6646)

```
Section 5.2 says:


   {

     "ietf-voucher:voucher": {

       "created-on": "2016-10-07T19:31:42Z",

       "expires-on": "2016-10-21T19:31:42Z",

       "assertion": "verified",

       "serial-number": "JADA123456789",

       "idevid-issuer": "base64encodedvalue==",

       "pinned-domain-cert": "base64encodedvalue==",

       "domain-cert-revocation-checks": "true",

       "last-renewal-date": "2017-10-07T19:31:42Z"

     }

   }

// state how to fix the above text here

```

## Issue description

The original JSON example contains a field that has a value of an incorrect data type, according to the YANG specification in section 5.3 of the same RFC 8366.
