# Errata 4450 - RFC 7273

- **RFC Title:** RTP Clock Source Signalling
- **RFC Publication Date:** June 2014

```
Section 4.8 says:


  ; PTP domain allowed characters: 0x21-0x7E (IEEE 1588-2002)

   ptp-domain-name = "domain-name=" 1*16ptp-domain-char

   ptp-domain-char = %x21-7E



   ; PTP domain allowed number range: 0-127 (IEEE 1588-2008)

   ptp-domain-nmbr = "domain-nmbr=" ptp-domain-dgts

   ptp-domain-dgts = ptp-domain-n1 / ptp-domain-n2 / ptp-domain-n3

   ptp-domain-n1   = DIGIT             ; 0-9

   ptp-domain-n2   = POS-DIGIT DIGIT   ; 10-99

   ptp-domain-n3   = ("10"/"11") DIGIT ; 100-119

                   / "12" %x30-37      ; 120-127

// state how to fix the above text here

Notes:

There is an inconsistency between ABNF in section 4.8 and examples in section 5.5.
```

## Issue description

The ABNF definitions in Section 4.8 of RFC 7273 for `ptp-domain-name` and `ptp-domain-nmbr` are inconsistent with the examples in Section 5.5 and with how existing implementations behave, making strict conformance to the ABNF as written impractical.
