# Errata 4212 - RFC 7366

- **RFC Title:** Encrypt-then-MAC for Transport Layer Security (TLS) and Datagram Transport Layer Security (DTLS)
- **RFC Publication Date:** September 2014
- Link to original errata report: [rfc-editor.org/errata/eid4212](https://www.rfc-editor.org/errata/eid4212)

```
Section 3 says:


   In TLS [2] notation, the MAC calculation for TLS 1.0 without

   the explicit Initialization Vector (IV) is:



   MAC(MAC_write_key, seq_num +

       TLSCipherText.type +

       TLSCipherText.version +

       TLSCipherText.length +

       ENC(content + padding + padding_length));



   and for TLS 1.1 and greater with an explicit IV is:



   MAC(MAC_write_key, seq_num +

       TLSCipherText.type +

       TLSCipherText.version +

       TLSCipherText.length +

       IV +

       ENC(content + padding + padding_length));


// state how to fix the above text here
```

## Issue description

Section 3 of RFC 7366 specifies MAC calculation formulas for TLS, but the text is ambiguous about which length value should be used in the computation. This ambiguity has led different implementers to reach different conclusions, causing interoperability issues between TLS implementations.
