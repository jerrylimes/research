# Errata 5049 - RFC 8078

- **RFC Title:** Managing DS Records from the Parent via CDS/CDNSKEY
- **RFC Publication Date:** March 2017

```
Section 4 says:


   The contents of the CDS or CDNSKEY RRset MUST contain one RR and only

   contain the exact fields as shown below.



      CDS 0 0 0 0



      CDNSKEY 0 3 0 0



   The keying material payload is represented by a single 0.  This

   record is signed in the same way as regular CDS/CDNSKEY RRsets are

   signed.



   Strictly speaking, the CDS record could be "CDS X 0 X 0" as only the

   DNSKEY algorithm is what signals the DELETE operation, but for

   clarity, the "0 0 0 0" notation is mandated -- this is not a

   definition of DS digest algorithm 0.  The same argument applies to

   "CDNSKEY 0 3 0 0"; the value 3 in the second field is mandated by

   [RFC4034], Section 2.1.2.

// state how to fix the above text here

Notes:

RFC 7344 defines both CDS and CDNSKEY record wire and presentation format to be identical to DS and DNSKEY wire and presentation format defined in RFC 4034.


```

## Issue description

Both the CDS and CDNSKEY records in Section 4 of RFC 8078 are contradicting their definition in RFC 4034, the CDS one in Section 2.2 of that RFC and the CDNSKEY one in Section 2.1.2. These are not stylistic changes but changes to the specifications' technical requirements, resulting in inconsistencies between the example and proper implementation.
