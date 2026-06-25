# Errata 5489 - RFC 7950

- **RFC Title:** The YANG 1.1 Data Modeling Language
- **RFC Publication Date:** August 2016

```
Section 7.20.3.2 says:


The argument "delete" deletes properties from the target node.  The

   properties to delete are identified by substatements to the "delete"

   statement. 

```

## Issue description

Section 7.20.3.2 does not correctly describe how to identify properties that need to be deleted. This is a direct contradiction within the specification impacting implementation. The text instructs the use of a non-existent mechanism, resulting in an inconsistent specification.
