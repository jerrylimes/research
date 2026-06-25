# Errata 5374 - RFC 8373

- **RFC Title:** Negotiating Human Language in Real-Time Communications
- **RFC Publication Date:** May 2018

```
Section 5.4. says:


   An offer or answer indicating written Greek both ways:



      m=text 45020 RTP/AVP 103 104

      a=hlang-send:gr

      a=hlang-recv:gr

// state how to fix the above text here

```

## Issue description

The original example uses the incorrect language tag for Greek according to the IANA language subtag registry. This inconsistency affects the interoperability of implementations that rely on the example to represent the Greek language.
