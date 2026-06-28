# Errata 5768 - RFC 7170

- **RFC Title:** Tunnel Extensible Authentication Protocol (TEAP) Version 1
- **RFC Publication Date:** May 2014

```
Section 5. says:


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

The potentially variable length of the MAC function output in Section 5 is inconsistent with the length of the Compound MAC (20 octets as defined in Section 4.2.13).  This inconsistency would cause implementations to fail unless the MAC output is truncated to 20 octets, which is not explicitly stated in the original specification.
