# Errata 4517 - RFC 7203

- **RFC Title:** An Incident Object Description Exchange Format (IODEF) Extension for Structured Cybersecurity Information
- **RFC Publication Date:** April 2014

```
Section 5.2 says:


The schema has the <sequence> </sequence> tags.

// state how to fix the above text here

```

## Issue description

The XML schema in Section 5.2 of RFC 7203 uses a tag form that is inconsistent with the examples elsewhere in the document, making the schema invalid and unparseable by standard XML schema validators. This directly impacts any implementation that relies on schema validation.
