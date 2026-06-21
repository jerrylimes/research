# Errata 5986 - RFC 7940

- **RFC Title:** Representing Label Generation Rulesets Using XML
- **RFC Publication Date:** August 2016
- Link to original errata report: [rfc-editor.org/errata/eid5986](https://www.rfc-editor.org/errata/eid5986)

```
Section 6.3.1 says:


   A simple rule to match a label where all characters are members of

   some class called "preferred-codepoint":          



       <rule name="preferred-label">

           <start />

           <class by-ref="preferred-codepoint" count="1"/>

           <end />

       </rule>

// state how to fix the above text here

```

## Issue description

The applicability of the specification of the rule contadicts the applicability outlined in its description. This inconsistency would lead to implementations incorrectly matching labels based on the length.
