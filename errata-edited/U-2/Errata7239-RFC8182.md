# Errata 7239 - RFC 8182

- **RFC Title:** The RPKI Repository Delta Protocol (RRDP)
- **RFC Publication Date:** July 2017

```
Section 3.2 says:


Certificate Authorities that use RRDP MUST include an instance of an

SIA AccessDescription extension in resource certificates they

produce, in addition to the ones defined in [RFC6487]:

// state how to fix the above text here

```

## Issue description

The original text is ambiguous about the type of certificate that should contain the SIA extension containing the id-ad-rpkiNotify accessMethod. This ambiguity led to different interpretations and implementations.
