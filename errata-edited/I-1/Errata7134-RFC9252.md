# Errata 7134 - RFC 9252

- **RFC Title:** BGP Overlay Services Based on Segment Routing over IPv6 (SRv6)
- **RFC Publication Date:** July 2022

```
Section 6.4 says:


                  +---------------------------------------+

                  |  RD (8 octets)                        |

                  +---------------------------------------+

                  |  Ethernet Tag ID (4 octets)           |

                  +---------------------------------------+

                  |  IP Address Length (1 octet)          |

                  +---------------------------------------+

                  |  Originating Router's IP Address      |

                  |          (4 or 16 octets)             |

                  +---------------------------------------+



                        Figure 10: EVPN Route Type 4

// state how to fix the above text here

```

## Issue description

The original figure uses the incorrect field name and size for one of the fields of EVPN Route Type 4. This inconsistency should be corrected to reflect the correct encoding of EVPN Route Type 4.
