# Errata 4865 - RFC 7598

- **RFC Title:** DHCPv6 Options for Configuration of Softwire Address and Port-Mapped Clients
- **RFC Publication Date:** July 2015
- Link to original errata report: [rfc-editor.org/errata/eid4865](https://www.rfc-editor.org/errata/eid4865)

```
Section 4.3 says:


dmr-prefix6-len: 8 bits long; expresses the bitmask length of the 

IPv6 prefix specified in the dmr-ipv6-prefix field.  Allowed

values range from 0 to 128.

// state how to fix the above text here

```

## Issue description

Section 4.3 of RFC 7598 contains a contradiction between this specification in that section and RFC 7599. This inconsistency needs to be resolved to ensure that implementations conform to both specifications. The corrected range is consistent with RFC 7599.
