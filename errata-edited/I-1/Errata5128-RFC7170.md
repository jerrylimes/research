# Errata 5128 - RFC 7170

- **RFC Title:** Tunnel Extensible Authentication Protocol (TEAP) Version 1
- **RFC Publication Date:** May 2014
- Link to original errata report: [rfc-editor.org/errata/eid5128](https://www.rfc-editor.org/errata/eid5128)

```
Section 5.2. says:


IMCK[j] = TLS-PRF(S-IMCK[j-1], "Inner Methods Compound Keys",

                IMSK[j], 60)


// state how to fix the above text here

```

## Issue description

The syntax of the TLS-PRF part of the IMCK[j] formula in Section 5.2 is incorrect according to the syntax of PRF in Section 5 of RFC5246. This inconsistency would lead to an incorrect calculation of IMCK[j], affecting the security of TEAP.
