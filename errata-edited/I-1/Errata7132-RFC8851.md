# Errata 7132 - RFC 8851

- **RFC Title:** RTP Payload Format Restrictions
- **RFC Publication Date:** January 2021

```
Section 10 says:


rid-id            = 1*(alpha-numeric / "-" / "_")

// state how to fix the above text here

```

## Issue description

The original ABNF for rid-id is inconsistent the rules for the RtpStreamId/RepairedRtpStreamId SDES from RFC 8852 section 3.
