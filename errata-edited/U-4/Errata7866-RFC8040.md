# Errata 7866 - RFC 8040

- **RFC Title:** RESTCONF Protocol
- **RFC Publication Date:** January 2017

```
Section Multiple says:


Text occurs in three places



1)    Section 3.5.3



      The leaf-list value is specified as a string, using the canonical

      representation for the YANG data type.  Any reserved characters

      MUST be percent-encoded, according to Sections 2.1 and 2.5 of

      [RFC3986].





2)    Section 3.5.3



      The key value is specified as a string, using the canonical

      representation for the YANG data type.  Any reserved characters

      MUST be percent-encoded, according to Sections 2.1 and 2.5 of

      [RFC3986]. 





3)    Section 5.1



      The contents of any query parameter value MUST be encoded according

      to Section 3.4 of [RFC3986].  Any reserved characters MUST be

      percent-encoded, according to Sections 2.1 and 2.5 of [RFC3986].

// state how to fix the above text here

```

## Issue description

The specification inconsistently refers to sections of RFC3986 for percent-encoding rules. The RFC 3986 references cited in all three locations in the original text are incomplete for their stated purpose.
