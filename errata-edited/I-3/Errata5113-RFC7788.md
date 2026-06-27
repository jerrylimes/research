# Errata 5113 - RFC 7788

- **RFC Title:** Home Networking Control Protocol
- **RFC Publication Date:** April 2016

```
Section 10 says:


10.2.2.  DHCPv6-Data TLV



    0                   1                   2                   3

    0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1

   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

   |    Type: DHCPv6-Data (37)     |          Length: > 0          |

   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+



[...]



10.2.3.  DHCPv4-Data TLV



    0                   1                   2                   3

    0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1

   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

   |     Type: DHCPv4-Data (38)    |          Length: > 0          |

   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

// state how to fix the above text here

```

## Issue description

The Type values for two TLVs are incorrect in Section 10. This inconsistency is between the values shown in Section 10 and the values defined in Section 13 and the IANA registry. This inconsistency would affect implementations parsing or generating these TLVs.
