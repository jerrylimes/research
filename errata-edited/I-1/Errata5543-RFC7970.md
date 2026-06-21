# Errata 5543 - RFC 7970

- **RFC Title:** The Incident Object Description Exchange Format Version 2
- **RFC Publication Date:** November 2016
- Link to original errata report: [rfc-editor.org/errata/eid5543](https://www.rfc-editor.org/errata/eid5543)

```
Section 8 says:


    <xs:element name="Confidence">

      <xs:complexType>

        <xs:attribute name="rating"

                      type="confidence-rating-type" use="required"/>

        <xs:attribute name="ext-rating"

                      type="xs:string" use="optional"/>

      </xs:complexType>

    </xs:element>

// state how to fix the above text here

```

## Issue description

The original schema definition for the Confidence element does not allow for a numerical value, while Section 3.12.5 specifies that a numerical assessment of confidence is possible. This inconsistency would prevent implementations from correctly handling numerical confidence values.
