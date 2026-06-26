# Errata 7955 - RFC 9562

- **RFC Title:** Universally Unique IDentifiers (UUIDs)
- **RFC Publication Date:** May 2024

```
Section 5.1 says:


time_high:

    The least significant 12 bits from the 60-bit starting timestamp.

    Occupies bits 52 through 63 (octets 6-7).

// state how to fix the above text here

```

## Issue description

The original text incorrectly describes what bits are supposed to be used in the time_high field. This inconsistency could lead to incorrect generation of UUIDs.
