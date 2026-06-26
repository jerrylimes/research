# Errata 8166 - RFC 8888

- **RFC Title:** RTP Control Protocol (RTCP) Feedback for Congestion Control
- **RFC Publication Date:** January 2021

```
Section 3.1 says:


         Following this, the report block contains a

   16-bit packet metric block for each RTP packet that has a sequence

   number in the range begin_seq to begin_seq+num_reports inclusive

   (calculated using arithmetic modulo 65536 to account for possible

   sequence number wrap-around).

// state how to fix the above text here

```

## Issue description

The text's description of the sequence number range as a closed interval is inconsistent with the format of an empty report and how the sequence numbers are used in reality.
