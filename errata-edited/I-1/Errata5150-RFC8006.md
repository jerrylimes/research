# Errata 5150 - RFC 8006

- **RFC Title:** Content Delivery Network Interconnection (CDNI) Metadata
- **RFC Publication Date:** December 2016
- Link to original errata report: [rfc-editor.org/errata/eid5150](https://www.rfc-editor.org/errata/eid5150)

```
Section 6.10 says:


         "generic-metadata-type": "MI.SourceMetadata",

         "generic-metadata-value": {

           "sources": [

             {

               "endpoint": ["acq1.ucdn.example"],

               "protocol": "http/1.1"

             },

             {

               "endpoint": ["acq2.ucdn.example"],

               "protocol": "http/1.1"

             }

           ]

         }


// state how to fix the above text here
```

## Issue description

A property name used in Section 6.10 of RFC 8006 fails to follow the grammar of property names in other sections like Section 4.2.1 and 4.2.1.1. This inconsistency directly relates to implementation as it affects how the SourceMetadata object should be structured and parsed, causing ambiguity in the implementation.
