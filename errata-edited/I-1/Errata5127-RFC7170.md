# Errata 5127 - RFC 7170

- **RFC Title:** Tunnel Extensible Authentication Protocol (TEAP) Version 1
- **RFC Publication Date:** May 2014
- Link to original errata report: [rfc-editor.org/errata/eid5127](https://www.rfc-editor.org/errata/eid5127)

```
Section 5.2. says:


IMSK = First 32 octets of TLS-PRF(EMSK, "TEAPbindkey@ietf.org" |

     "\0" | 64)

// state how to fix the above text here

```

## Issue description

Section 5.2 presents a contradiction between its TLS-PRF specification and the one in Section 5 of RFC 5246. This inconsistency can lead to incorrect IMSK generation, affecting the security of the TEAP protocol.
