# Errata 7657 - RFC 8006

- **RFC Title:** Content Delivery Network Interconnection (CDNI) Metadata
- **RFC Publication Date:** December 2016
- Link to original errata report: [rfc-editor.org/errata/eid7657](https://www.rfc-editor.org/errata/eid7657)

```
Section 6.10 says:


   {

     "metadata": [

       {

         "generic-metadata-type": "MI.TimeWindowACL",

         "generic-metadata-value": {

           "times": [

             "windows": [

               {

                 "start": "1213948800",

                 "end": "1478047392"

               }

             ],

             "action": "allow"

           ]

         }

       }

     ]

   }

// state how to fix the above text here

```

## Issue description

A property in Section 6.10's JSON example contains a structural error. Also, a property is accepting a value of unmatched data type. This inconsistency makes the original example unimplementable without additional clarification.
