# Errata 5715 - RFC 8224

- **RFC Title:** Authenticated Identity Management in the Session Initiation Protocol (SIP)
- **RFC Publication Date:** February 2018

```
Section 4.1 says:


o  Second, the JSON "dest" array MUST be populated.  If the

   destination identity is a telephone number, then the array MUST be

   populated with a JSON object containing a "tn" element with a

   value set to the value of the quoted destination identity, a

   canonicalized telephone number (see Section 8.3).  Otherwise, the

   array MUST be populated with a JSON object containing a "uri"

   element, set to the value of the addr-spec component of the

   To header field, which is the AoR to which the request is being

   sent, per the procedures in Section 8.5.  Multiple JSON objects

   are permitted in "dest" for future compatibility reasons.



...



The "orig" and "dest" arrays may contain identifiers of heterogeneous

type; for example, the "orig" array might contain a "tn" claim, while

the "dest" contains a "uri" claim.  Also note that in some cases, the

"dest" array may be populated with more than one value.  This could,

for example, occur when multiple "dest" identities are specified in a

meshed conference.  Defining how a SIP implementation would align

multiple destination identities in PASSporT with such systems is left

as a subject for future specifications.

// state how to fix the above text here

```

## Issue description

The original description of the "dest" element as an "array" is inconsistent with Section 5.2.1 of RFC 8225 and the provided example.
