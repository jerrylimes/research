# Errata 7386 - RFC 8881

- **RFC Title:** Network File System (NFS) Version 4 Minor Version 1 Protocol
- **RFC Publication Date:** August 2020

```
Section 18.46.3. says:


                                                             Operations

   other than SEQUENCE, BIND_CONN_TO_SESSION, EXCHANGE_ID,

   CREATE_SESSION, and DESTROY_SESSION, MUST NOT appear as the first

   operation in a COMPOUND.

// state how to fix the above text here

```

## Issue description

The original text does not take texts in Section 18.50.3 that describes an operation into consideration. This discrepancy creates an inconsistency between the general rule and the specific exception for this operation.
