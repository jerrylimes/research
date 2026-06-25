# Errata 6385 - RFC 8007

- **RFC Title:** Content Delivery Network Interconnection (CDNI) Control Interface / Triggers
- **RFC Publication Date:** December 2016

```
Section 4.1 says:


   When a CI/T Trigger Command is accepted, the uCDN MUST create a new

   Trigger Status Resource that will convey a specification of the CI/T

   Command and its current status.  The HTTP response to the dCDN MUST

   have status code 201 and MUST convey the URI of the Trigger Status

   Resource in the Location header field [RFC7231].

// state how to fix the above text here

```

## Issue description

The original text incorrectly describes the roles of the uCDN and dCDN when a CI/T Trigger Command is accepted. This inconsistency affects the understanding of the protocol's operation and the correct implementation of the interaction between the two CDNs.
