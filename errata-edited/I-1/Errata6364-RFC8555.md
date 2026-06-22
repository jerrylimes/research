# Errata 6364 - RFC 8555

- **RFC Title:** Automatic Certificate Management Environment (ACME)
- **RFC Publication Date:** March 2019
- Link to original errata report: [rfc-editor.org/errata/eid6364](https://www.rfc-editor.org/errata/eid6364)

```
Section 7.1.4 says:


   wildcard (optional, boolean):  This field MUST be present and true

      for authorizations created as a result of a newOrder request

      containing a DNS identifier with a value that was a wildcard

      domain name.  For other authorizations, it MUST be absent.

      Wildcard domain names are described in Section 7.1.3.

// state how to fix the above text here

```

## Issue description

The description of the `wildcard` field is not consistent with the provided example that follows it and lacks clarity in the handling of pre-authorizations.
