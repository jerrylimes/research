# Errata 8184 - RFC 9483

- **RFC Title:** Lightweight Certificate Management Protocol (CMP) Profile
- **RFC Publication Date:** November 2023

```
Section 4.1.6.2 says:


          rid           REQUIRED

-- MUST contain the subjectKeyIdentifier of the CMP protection

--   certificate, if available, in the rKeyId choice, and the

--   subjectKeyIdentifier MUST equal the senderKID in the

--   PKIHeader.

-- If the CMP protection certificate does not contain a

--   subjectKeyIdentifier, the issuerAndSerialNumber choice MUST

--   be used

// state how to fix the above text here

```

## Issue description

The original text does not clarify which CMP protection certificate to check for the subjectKeyIdentifier. It also contains an inaccurate normative statement about the relationship between `subjectKeyIdentifier` and `senderKID` in the PKIHeader.
