# Errata 5544 - RFC 7970

- **RFC Title:** The Incident Object Description Exchange Format Version 2
- **RFC Publication Date:** November 2016

```
Section 8 says:


 <xs:element name="Node">

      <xs:complexType>

        <xs:sequence>

          <xs:choice maxOccurs="unbounded">

            <xs:element ref="iodef:DomainData"

                        minOccurs="0" maxOccurs="unbounded"/>

            <xs:element ref="iodef:Address"

                        minOccurs="0" maxOccurs="unbounded"/>

          </xs:choice>

          <xs:element ref="iodef:PostalAddress" minOccurs="0"/>

          <xs:element ref="iodef:Location"

                      minOccurs="0" maxOccurs="unbounded"/>

          <xs:element ref="iodef:Counter"

                      minOccurs="0" maxOccurs="unbounded"/>

        </xs:sequence>

      </xs:complexType>

    </xs:element>

// state how to fix the above text here

```

## Issue description

Section 3.18 requires at least one of the DomainData and Address elements need to be presented, but Section 8's implementation does not follow this requirement.
