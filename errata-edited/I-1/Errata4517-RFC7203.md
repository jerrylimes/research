# Errata 4517 - RFC 7203

- **RFC Title:** An Incident Object Description Exchange Format (IODEF) Extension for Structured Cybersecurity Information
- **RFC Publication Date:** April 2014
- Link to original errata report: [rfc-editor.org/errata/eid4517](https://www.rfc-editor.org/errata/eid4517)

```
Section 5.2 says:


The schema has the <sequence> </sequence> tags.

// state how to fix the above text here

```

## Issue description

The erratum corrects an error in the schema definition. This inconsistency directly impacts the usability of the schema as it cannot be parsed by schema validators, affecting implementations that rely on schema validation.
