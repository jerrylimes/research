# Errata 5078 - RFC 7252

- **RFC Title:** The Constrained Application Protocol (CoAP)
- **RFC Publication Date:** June 2014
- Link to original errata report: [rfc-editor.org/errata/eid5078](https://www.rfc-editor.org/errata/eid5078)

```
Section 7.2.1 says:


The Content-Format code

attribute MAY include a space-separated sequence of Content-Format

codes, indicating that multiple content-formats are available.  The

syntax of the attribute value is summarized in the production "ct-

value" in Figure 12, where "cardinal", "SP", and "DQUOTE" are defined

as in [RFC6690].

// state how to fix the above text here

```

## Issue description

The original text does not what the space-separated sequence implies into consideration. This creates an inconsistency and ambiguity in how the Content-Format attribute should be used.
