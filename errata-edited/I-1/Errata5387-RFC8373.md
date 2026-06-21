# Errata 5387 - RFC 8373

- **RFC Title:** Negotiating Human Language in Real-Time Communications
- **RFC Publication Date:** May 2018
- Link to original errata report: [rfc-editor.org/errata/eid5387](https://www.rfc-editor.org/errata/eid5387)

```
Section 5.4. says:


      m=text 45020 RTP/AVP 103 104

      a=hlang-send:sp pt



      m=audio 49250 RTP/AVP 20

      a=hlang-recv:sp pt



   An answer for the above offer, indicating text in which the callee

   will receive written Spanish and audio in which the callee will send

   spoken Spanish.  (The answering party has no video capability):



      m=video 0 RTP/AVP 31 32

      m=text 45020 RTP/AVP 103 104

      a=hlang-recv:sp



      m=audio 49250 RTP/AVP 20

      a=hlang-send:sp



and later on the same page:



   An answer for the above offer, indicating text in which the callee

   will receive written Spanish, audio in which the callee will send

   spoken Spanish, and supplemental video:



      m=text 45020 RTP/AVP 103 104

      a=hlang-recv:sp



      m=audio 49250 RTP/AVP 20

      a=hlang-send:sp



      m=video 51372 RTP/AVP 31 32

// state how to fix the above text here

```

## Issue description

The original example uses the incorrect language tag for Spanish according to the IANA language subtag registry. This inconsistency affects the interoperability of implementations that rely on the examples to represent the Spanish language.
