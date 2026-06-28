# Errata 6752 - RFC 9134

- **RFC Title:** RTP Payload Format for ISO/IEC 21122 (JPEG XS)
- **RFC Publication Date:** October 2021

```
Section 4.2 says:


As specified in [RFC3550] and [RFC4175], the RTP timestamp

designates the sampling instant of the first octet of the video

frame to which the RTP packet belongs.  Packets SHALL NOT include

data from multiple video frames, and all packets belonging to the

same video frame SHALL have the same timestamp.  Several

successive RTP packets will consequently have equal timestamps if

they belong to the same video frame (that is until the marker bit

is set to 1, marking the last packet of the video frame), and the

timestamp is only increased when a new video frame begins.

// state how to fix the above text here

```

## Issue description

The original text is unclear about whether the RTP timestamp applies to video frames or fields.
