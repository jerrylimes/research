# Errata 7654 - RFC 8955

- **RFC Title:** Dissemination of Flow Specification Rules
- **RFC Publication Date:** December 2020

```
Section 4 says:


   This NLRI information is encoded using MP_REACH_NLRI and

   MP_UNREACH_NLRI attributes, as defined in [RFC4760].  When

   advertising Flow Specifications, the Length of the Next-Hop Network

   Address MUST be set to 0.  The Network Address of the Next-Hop field

   MUST be ignored.

// state how to fix the above text here

```

## Issue description

The original text creates ambiguity by using incorrect field names for the Next Hop Network Address attributes. This inconsistency could lead to implementations incorrectly handling the Next Hop Network Address attributes when advertising Flow Specifications.
