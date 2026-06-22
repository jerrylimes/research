# Errata 6842 - RFC 8561

- **RFC Title:** A YANG Data Model for Microwave Radio Link
- **RFC Publication Date:** June 2019
- Link to original errata report: [rfc-editor.org/errata/eid6842](https://www.rfc-editor.org/errata/eid6842)

```
Section Annex A.3 says:


 "name": "RLT-A:CT-2",

...

           "tx-frequency": 10618000,

// state how to fix the above text here

```

## Issue description

The original example contains a typo for the XPIC configuration that makes the configuration incosistent with A.2. This inconsistency would lead to implementations misinterpreting the example configuration.
