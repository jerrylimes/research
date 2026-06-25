# Errata 5870 - RFC 8360

- **RFC Title:** Resource Public Key Infrastructure (RPKI) Validation Reconsidered
- **RFC Publication Date:** April 2018

```
Section 4.2.3 says:


       ext-pe-autonomousSysIds-v2 EXTENSION ::= {

         SYNTAX ASIdentifiers

         IDENTIFIED BY id-pe-autonomousSysIds-v2

       }



       id-pe-autonomousSysIds OBJECT IDENTIFIER ::= { id-pe 29 }

// state how to fix the above text here

```

## Issue description

The original ASN.1 definition is using an incorrect information object in the OBJECT IDENTIFIER, which is necessary for correct compilation and consistency with the EXTENSION definition.
