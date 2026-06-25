# Errata 7094 - RFC 95

- **RFC Title:** JSON Responses for the Registration Data Access Protocol (RDAP)
- **RFC Publication Date:** June 2021

```
Section 2.1 says:


If The Registry of the Moon desires to express information not found

in this specification, it might select "lunarNIC" as its identifying

prefix and insert, as an example, the member named

"lunarNIC_beforeOneSmallStep" to signify registrations occurring

before the first moon landing and the member named

"lunarNIC_harshMistressNotes" that contains other descriptive text.



Consider the following JSON response with JSON names, some of which

should be ignored by clients without knowledge of their meaning.



{

  "handle" : "ABC123",

  "lunarNIC_beforeOneSmallStep" : "TRUE THAT!",

  "remarks" :

  [

    {

      "description" :

      [

        "She sells sea shells down by the sea shore.",

        "Originally written by Terry Sullivan."

      ]

    }

  ],

  "lunarNIC_harshMistressNotes" :

  [

    "In space,",

    "nobody can hear you scream."

  ]

}

Figure 2

// state how to fix the above text here

```

## Issue description

The original example uses a string identifier that is inconsistent with the example in Section 4.1. This inconsistency can cause significant misunderstanding of the technical specification and might result in faulty implementations if not corrected.
