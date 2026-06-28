# Errata 4413 - RFC 7584

- **RFC Title:** Session Traversal Utilities for NAT (STUN) Message Handling for SIP Back-to-Back User Agents (B2BUAs)
- **RFC Publication Date:** July 2015

```
Section 4.4 says:


   Because of forking, a B2BUA might receive multiple answers for a

   single outbound INVITE.  When this occurs, the B2BUA SHOULD follow

   Sections 3.2 or 3.3 for all of those received answers.

// state how to fix the above text here

```

## Issue description

The original text refers to non-existent sections (3.2 and 3.3) for handling multiple INVITE answers. This inconsistency would mislead implementations attempting to correctly handle multiple INVITE answers.

**For this example, the correct fix has been provided to you as a guide to how to correctly disambiguate the erroneous text.**

## Correct fix

```
It should say:

   Because of forking, a B2BUA might receive multiple answers for a

   single outbound INVITE.  When this occurs, the B2BUA SHOULD follow

   Sections 4.2 or 4.3 for all of those received answers.
```
