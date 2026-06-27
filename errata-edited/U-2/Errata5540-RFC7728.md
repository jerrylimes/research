# Errata 5540 - RFC 7728

- **RFC Title:** RTP Stream Pause and Resume
- **RFC Publication Date:** February 2016

```
Section 8.2.  PAUSED says:


   PAUSED SHALL contain a fixed-length 32-bit parameter at the start of

   the Type Specific field with the extended RTP sequence number of the

   last RTP packet sent before the RTP stream was paused, in the same

   format as the extended highest sequence number received

   (Section 6.4.1 of [RFC3550]).

// state how to fix the above text here

```

## Issue description

The original specification does not define the value of the 32-bit parameter in the PAUSED message when no RTP packets have been sent before pausing. This under-specification leads to ambiguity in implementations and potential interoperability issues.
