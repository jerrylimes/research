# Errata 7822 - RFC 9480

- **RFC Title:** Certificate Management Protocol (CMP) Updates
- **RFC Publication Date:** November 2023

```
Section A.2 says:


PKIHeader ::= SEQUENCE {

       pvno                INTEGER     { cmp1999(1), cmp2000(2),

                                         cmp2012(3) },

// state how to fix the above text here

```

## Issue description

The original ASN.1 module contains a typo that uses the incorrect version number for the CMP protocol. This inconsistency would affect implementations that rely on the correct version number for processing CMP messages.
