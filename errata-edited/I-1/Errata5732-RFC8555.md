# Errata 5732 - RFC 8555

- **RFC Title:** Automatic Certificate Management Environment (ACME)
- **RFC Publication Date:** March 2019
- Link to original errata report: [rfc-editor.org/errata/eid5732](https://www.rfc-editor.org/errata/eid5732)

```
Section 8 says:


A challenge object with an error MUST have status

equal to "invalid".

// state how to fix the above text here

```

## Issue description

The statement in Section 8 that a challenge object with an error MUST have status equal to "invalid" is inconsistent with the retry mechanism described in Section 8.2.
