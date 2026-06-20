# Errata 4297 - RFC 7394

- **RFC Title:** Definition of Time to Live TLV for LSP-Ping Mechanisms
- **RFC Publication Date:** November 2014
- Link to original errata report: [rfc-editor.org/errata/eid4297](https://www.rfc-editor.org/errata/eid4297)

```
Section 3.1 says:


3.1. TTL TLV Format





   0                   1                   2                   3

   0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1

   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

   |  Type = 32769                 |   Length = 8                  |

   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

   |   Value       |   Reserved    |   Flags                       |

   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+



                  Figure 1: Time To Live TLV Format
// state how to fix the above text here
```

## Issue description

The TTL TLV format diagram in Section 3.1 of RFC 7394 specifies a field value that conflicts with how RFC 4379 defines TLV Length fields, leading to incorrect interpretation of the TTL TLV by implementations.
