# Errata 7986 - RFC 95

- **RFC Title:** JSON Responses for the Registration Data Access Protocol (RDAP)
- **RFC Publication Date:** June 2021
- Link to original errata report: [rfc-editor.org/errata/eid7986](https://www.rfc-editor.org/errata/eid7986)

```
Section 9 says:


The following is an elided example of an entity truncated data.



{

  "objectClassName" : "entity",

  "handle" : "ANENTITY",

  "roles" : [ "registrant" ],

  ...

  "entities" :

  [

    {

      "objectClassName" : "entity",

      "handle": "ANEMBEDDEDENTITY",

      "roles" : [ "technical" ],

      ...

    },

    ...

  ],

  "networks" :

  [

    ...

  ],

  ...

  "remarks" :

  [

    {

      "title" : "Data Policy",

      "type" : "object truncated due to unexplainable reason",

      "description" :

      [

        "Some of the data in this object has been removed."

      ],

      "links" :

      [

        {

          "value" : "https://example.net/help",

          "rel" : "alternate",

          "type" : "text/html",

          "href" : "https://www.example.com/data_policy.html"

        }

      ]

    }

  ]

}

// state how to fix the above text here

```

## Issue description

The example JSON response in Section 9 omits a property that is required in Section 4.1 of RFC9083, creating an inconsistency between the example and the specification.
