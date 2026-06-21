# Errata 5791 - RFC 8620

- **RFC Title:** The JSON Meta Application Protocol (JMAP)
- **RFC Publication Date:** July 2019
- Link to original errata report: [rfc-editor.org/errata/eid5791](https://www.rfc-editor.org/errata/eid5791)

```
Section 2.1 says:


"capabilities": {

  "urn:ietf:params:jmap:core": {

    "maxSizeUpload": 50000000,

    "maxConcurrentUpload": 8,

    "maxSizeRequest": 10000000,

    "maxConcurrentRequest": 8,

    "maxCallsInRequest": 32,

    "maxObjectsInGet": 256,

    "maxObjectsInSet": 128,

    "collationAlgorithms": [

      "i;ascii-numeric",

      "i;ascii-casemap",

      "i;unicode-casemap"

    ]

  },

  "urn:ietf:params:jmap:mail": {}

  "urn:ietf:params:jmap:contacts": {},

  "https://example.com/apis/foobar": {

    "maxFoosFinangled": 42

  }

}

// state how to fix the above text here

```

## Issue description

A punctuation is missing, and a property name is grammatically incorrect. This inconsistency would cause issues when parsing and generating JMAP capability responses.
