# Errata 5844 - RFC 7170

- **RFC Title:** Tunnel Extensible Authentication Protocol (TEAP) Version 1
- **RFC Publication Date:** May 2014
- Link to original errata report: [rfc-editor.org/errata/eid5844](https://www.rfc-editor.org/errata/eid5844)

```
Section C.1 says:


                            <- Crypto-Binding TLV (Request),

                                Result TLV (Success),

                                (Optional PAC TLV)



       Crypto-Binding TLV(Response),

       Result TLV (Success),

       (PAC-Acknowledgement TLV) ->

// state how to fix the above text here

```

## Issue description

The example message sequence in Section C.1 does not include what is implied to be used in the sequence in Section 3.3.2. This inconsistency affects implementations that follow the example sequence literally but must also follow section 3.3.2.
