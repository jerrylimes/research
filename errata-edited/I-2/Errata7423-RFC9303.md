# Errata 7423 - RFC 9303

- **RFC Title:** Locator/ID Separation Protocol Security (LISP-SEC)
- **RFC Publication Date:** October 2022

```
Section 6.9 says:


ITR MUST set the 'EID HMAC ID' field to 0 before computing the HMAC.

// state how to fix the above text here

```

## Issue description

The original text refers to the incorrect field. This inconsistency would affect implementations computing the HMAC.
