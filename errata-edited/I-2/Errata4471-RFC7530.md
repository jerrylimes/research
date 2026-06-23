# Errata 4471 - RFC 7530

- **RFC Title:** Network File System (NFS) Version 4 Protocol
- **RFC Publication Date:** March 2015
- Link to original errata report: [rfc-editor.org/errata/eid4471](https://www.rfc-editor.org/errata/eid4471)

```
Section 16.10.4. says:


   In the case that the lock is denied, the owner, offset, and length of

   a conflicting lock are returned.

// state how to fix the above text here

```

## Issue description

The original description is missing out something that is necessary to match the description of LOCKT in section 16.11.4.
