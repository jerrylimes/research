# Errata 5436 - RFC 7208

- **RFC Title:** Sender Policy Framework (SPF) for Authorizing Use of Domains in Email, Version 1
- **RFC Publication Date:** April 2014

```
Throughout the document, when it says:


    header-field     = "Received-SPF:" [CFWS] result FWS [comment FWS]

                       [ key-value-list ] CRLF

// state how to fix the above text here

```

## Issue description

The original text does not allow a header field value like result-FWS-comment with no FWS or key-value-list following it. The original ABNF is too restrictive, preventing valid header field values from being parsed. This inconsistency impacts implementations that parse Received-SPF header fields, leading to potential errors in processing.
