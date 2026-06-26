# Errata 8183 - RFC 9483

- **RFC Title:** Lightweight Certificate Management Protocol (CMP) Profile
- **RFC Publication Date:** November 2023

```
Section 4.1.6.1 says:


              rid             REQUIRED

    -- MUST contain the subjectKeyIdentifier of the CMP protection

    --   certificate, if available, in the rKeyId choice, and the

    --   subjectKeyIdentifier MUST equal the senderKID in the

    --   PKIHeader.

    -- If the CMP protection certificate does not contain a

    --   subjectKeyIdentifier, the issuerAndSerialNumber choice MUST

    --   be used.

// state how to fix the above text here

```

## Issue description

The original text refers to the incorrect method for specifying the recipient identifier (rid), using the rKeyId choice which is not defined in Section 6.2.1 of RFC 5652. It also does not clarify which CMP protection certificate to check for the subjectKeyIdentifier.
