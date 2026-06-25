# Errata 5650 - RFC 8152

- **RFC Title:** CBOR Object Signing and Encryption (COSE)
- **RFC Publication Date:** July 2017

```
Section Section 13.2 says:


   | crv  | 1     | -1    | int /  | EC identifier - Taken from the    |

   |      |       |       | tstr   | "COSE Key Common Parameters"      |

   |      |       |       |        | registry                          |

// state how to fix the above text here

```

## Issue description

The original text points to the wrong registry for EC identifiers. This inconsistency could lead to incorrect interpretation and implementation.
