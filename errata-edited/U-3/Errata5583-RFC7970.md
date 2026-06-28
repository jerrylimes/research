# Errata 5583 - RFC 7970

- **RFC Title:** The Incident Object Description Exchange Format Version 2
- **RFC Publication Date:** November 2016
- Link to original errata report: [rfc-editor.org/errata/eid5583](https://www.rfc-editor.org/errata/eid5583)

```
Section 8 says:


    <xs:simpleType name="action-type">

      <xs:restriction base="xs:NMTOKEN">

        <xs:enumeration value="nothing"/>

        <xs:enumeration value="contact-source-site"/>

        <xs:enumeration value="contact-target-site"/>

        <xs:enumeration value="contact-sender"/>

        <xs:enumeration value="investigate"/>

        <xs:enumeration value="block-host"/>

        <xs:enumeration value="block-network"/>

        <xs:enumeration value="block-port"/>

        <xs:enumeration value="rate-limit-host"/>

        <xs:enumeration value="rate-limit-network"/>

        <xs:enumeration value="rate-limit-port"/>

        <xs:enumeration value="redirect-traffic"/>

        <xs:enumeration value="honeypot"/>

        <xs:enumeration value="upgrade-software"/>

        <xs:enumeration value="rebuild-asset"/>

        <xs:enumeration value="harden-asset"/>

        <xs:enumeration value="remediate-other"/>

        <xs:enumeration value="status-triage"/>

        <xs:enumeration value="status-new-info"/>

        <xs:enumeration value="watch-and-report"/>

        <xs:enumeration value="defined-coa"/>

// state how to fix the above text here

```

## Issue description

The original schema definition for the action-type is missing an enumeration value, which is defined in the narrative text in Section 3.1.5.
