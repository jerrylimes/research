# Errata 5775 - RFC 7170

- **RFC Title:** Tunnel Extensible Authentication Protocol (TEAP) Version 1
- **RFC Publication Date:** May 2014

```
Section 5. says:


   For authentication methods that generate keying material, further

   protection against man-in-the-middle attacks is provided through

   cryptographically binding keying material established by both TEAP

   Phase 1 and TEAP Phase 2 conversations.  After each successful inner

   EAP authentication, EAP EMSK and/or MSKs are cryptographically

   combined with key material from TEAP Phase 1 to generate a Compound

   Session Key (CMK).  The CMK is used to calculate the Compound MAC as

   part of the Crypto-Binding TLV described in Section 4.2.13, which

   helps provide assurance that the same entities are involved in all

   communications in TEAP.  During the calculation of the Compound MAC,

   the MAC field is filled with zeros.



   The Compound MAC computation is as follows:



      CMK = CMK[j]

      Compound-MAC = MAC( CMK, BUFFER )



   where j is the number of the last successfully executed inner EAP

   method, MAC is the MAC function negotiated in TLS 1.2 [RFC5246], and

   BUFFER is created after concatenating these fields in the following

   order:

// state how to fix the above text here

```

## Issue description

Section 5 does not specify how the CMK is derived when no inner EAP authentication method is executed. The lack of clear guidance on CMK derivation in this scenario directly affects the implementation's ability to generate correct Compound MAC values.
