# Errata 6940 - RFC 79

- **RFC Title:** Internet Key Exchange Protocol Version 2 (IKEv2)
- **RFC Publication Date:** October 2014
- Link to original errata report: [rfc-editor.org/errata/eid6940](https://www.rfc-editor.org/errata/eid6940)

```
Section .10 says:


o SPI Size (1 octet) - Length in octets of the SPI as defined by the

 IPsec protocol ID or zero if no SPI is applicable. For a

 notification concerning the IKE SA, the SPI Size MUST be zero and

 the field must be empty.


// state how to fix the above text here

```

## Issue Description

The original text is unclear on what the SPI should precisely be like for IKE SA notifications. It leaves room for misinterpretation.
