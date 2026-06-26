# Errata 8103 - RFC 9421

- **RFC Title:** HTTP Message Signatures
- **RFC Publication Date:** February 2024

```
Section 7.5.3 says:


Several parts of this specification rely on the parsing of Structured

Field values [STRUCTURED-FIELDS] -- in particular, strict

serialization of HTTP Structured Field values (Section 2.1.1),

referencing members of a Dictionary Structured Field (Section 2.1.2),

and processing the @signature-input value when verifying a signature

(Section 3.2).  While Structured Field values are designed to be

relatively simple to parse, a naive or broken implementation of such

a parser could lead to subtle attack surfaces being exposed in the

implementation.



For example, if a buggy parser of the @signature-input value does not

enforce proper closing of quotes around string values within the list

of component identifiers, an attacker could take advantage of this

and inject additional content into the signature base through

manipulating the Signature-Input field value on a message.

// state how to fix the above text here

```

## Issue description

The text in Section 7.5.3 contains an error in the description of one of the steps of parsing the Structured Field Values that could resulting in failure of signature verification.
