# Errata 8020 - RFC 9487

- **RFC Title:** Export of Segment Routing over IPv6 Information in IP Flow Information Export (IPFIX)
- **RFC Publication Date:** November 2023
- Link to original errata report: [rfc-editor.org/errata/eid8020](https://www.rfc-editor.org/errata/eid8020)

```
Section A.2 says:


Figure 7:



   0                   1                   2                   3

   0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1

+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

|         Set ID = 3            |          Length = 24          |

+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

|       Template ID 259         |        Field Count = 3        |

+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

|     Scope Field Count = 1     |0| srhActiveSegmentIPv6 = 495  |

+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

|   Scope 1 Field Length = 4    |0|srhSegmentIPv6End.Behav = 502|

+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

|       Field Length = 1        |0|srhSegmentIPv6Lo.Length = 501|

+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

|       Field Length = 4        |           Padding             |

+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+



Figure 8:



 0                   1                   2                   3

 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1

+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

|         SET ID = 259          |           Length = 28         |

+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

|               srhActiveSegmentIPv6 = 2001:db8::1              |

+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

|srhSegmentIPv6EndpointBehavior |srhSegmentIPv6LocatorLength= 48|

|= End [1]                      |                               |

+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

|               srhActiveSegmentIPv6 = 2001:db8::4              |

+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

|srhSegmentIPv6EndpointBehavior |srhSegmentIPv6LocatorLength= 48|

|= End with NEXT-CSID [43]      |                               |

+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

|               srhActiveSegmentIPv6 = 2001:db8::6              |

+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

|srhSegmentIPv6EndpointBehavior |srhSegmentIPv6LocatorLength= 48|

|= End.DX6 [16]                 |                               |

+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+







// state how to fix the above text here

```

## Explanation

The figures in Appendix A.2 use incorrect information element IDs that do not mirror Section 6.2's IPFIX option-template.
