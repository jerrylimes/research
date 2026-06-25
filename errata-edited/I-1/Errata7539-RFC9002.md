# Errata 7539 - RFC 9002

- **RFC Title:** QUIC Loss Detection and Congestion Control
- **RFC Publication Date:** May 2021

```
Section 5. says:


smoothed_rtt = 7/8 * smoothed_rtt + 1/8 * adjusted_rtt

rttvar_sample = abs(smoothed_rtt - adjusted_rtt)

rttvar = 3/4 * rttvar + 1/4 * rttvar_sample

// state how to fix the above text here

```

## Issue description

The original order of calculations is incorrect according to Appendix A.7 of this RFC and Section 2 of the referred RFC 6298. This inconsistency would result in incorrect RTT and RTT variance calculations.
