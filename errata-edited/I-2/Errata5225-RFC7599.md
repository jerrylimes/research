# Errata 5225 - RFC 7599

- **RFC Title:** Mapping of Address and Port using Translation (MAP-T)
- **RFC Publication Date:** July 2015

```
Section 6 says:


In the case of an IPv4 prefix, the IPv4 address field is right-padded

with zeros up to 32 bits.  The PSID is left-padded with zeros to

create a 16-bit field.  For an IPv4 prefix or a complete IPv4

address, the PSID field is zero.

// state how to fix the above text here

```

## Issue description

The original description for MAP-T contains information that is only applicable to MAP-E. This inconsistency is due to the text being copied from MAP-E where it is correct, but incorrect for MAP-T.
