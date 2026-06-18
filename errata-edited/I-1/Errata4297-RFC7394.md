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

The original specification incorrectly defines one of the fields. The correction should align with RFC 4379. This inconsistency would lead to incorrect interpretation and processing of the Time To Live TLV.
