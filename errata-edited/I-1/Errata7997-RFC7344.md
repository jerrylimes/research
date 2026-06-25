# Errata 7997 - RFC 7344

- **RFC Title:** Automating DNSSEC Delegation Trust Maintenance
- **RFC Publication Date:** September 2014

```
Section 6.2.1 says:


When a Parent operates in "calculate DS" mode, it can operate in one

   of two sub-modes:



   full:  The Parent only publishes DS records it calculates from DNSKEY

      records.

// state how to fix the above text here

```

## Issue description

The description of the "full" submode in Section 6.2.1 is incorrect. This is an inconsistency that directly affects the implementation of the specification.
