# Errata 8199 - RFC 8972

- **RFC Title:** Simple Two-Way Active Measurement Protocol Optional Extensions
- **RFC Publication Date:** January 2021

```
Section 4.4 says:


Also, the Session-Reflector MUST copy the value of the DSCP and ECN

fields of the IP header of the received STAMP test packet into the

DSCP2 field in the reflected test packet.

// state how to fix the above text here

Notes:

First, thank you to all the IETF contributors who do such amazing work to keep the Internet going (seriously!). I noticed this minor omission while implementing the specification. I spoke with Mr. Mirsky (one of the authors) who suggested I file this report. Of course, the authors' intent is not in doubt, but he suggested that I submit this report nonetheless. Besides this very minor misstatement, as someone writing an implementation who was completely uninvolved in drafting the RFC, I have found this document to be incredibly readable and easy to follow -- thank you!


[Edit: WK (Ops AD): Thanks for the Errata (and the kind note) ].
```

## Issue description

The original text copies the value of two fields into one, which is illogical.
