# Errata 7384 - RFC 8410

- **RFC Title:** Algorithm Identifiers for Ed25519, Ed448, X25519, and X448 for Use in the Internet X.509 Public Key Infrastructure
- **RFC Publication Date:** August 2018

```
Section 9 says:


    sa-Ed25519 SIGNATURE-ALGORITHM ::= {

       IDENTIFIER id-Ed25519

        PARAMS ARE absent

        PUBLIC-KEYS {pk-Ed25519}

        SMIME-CAPS { IDENTIFIED BY id-Ed25519 }

    }



    pk-Ed25519 PUBLIC-KEY ::= {

        IDENTIFIER id-Ed25519

        -- KEY no ASN.1 wrapping --

        PARAMS ARE absent

        CERT-KEY-USAGE {digitalSignature, nonRepudiation,

                        keyCertSign, cRLSign}

        PRIVATE-KEY CurvePrivateKey

    }

// state how to fix the above text here

```

## Issue description

The original specification is missing two object assignment definitions that are implied by the document's stated scope, creating an inconsistency between the algorithms covered elsewhere in the RFC and those present in this section.
