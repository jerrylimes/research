# Errata 7020 - RFC 7951

- **RFC Title:** JSON Encoding of Data Modeled with YANG
- **RFC Publication Date:** August 2016

```
Section 6.8 says:


An "identityref" value is represented as a string -- the name of an

identity.  If the identity is defined in a module other than the leaf

node containing the identityref value, the namespace-qualified form

(Section 4) MUST be used.  Otherwise, both the simple and namespace-

qualified forms are permitted.

// state how to fix the above text here

```

## Issue description

The original text does not consider all the possible nodes that can be of "identityref" type. This omission creates an inconsistency between the description and the actual permissible usage.
