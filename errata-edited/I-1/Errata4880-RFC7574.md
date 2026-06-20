# Errata 4880 - RFC 7574

- **RFC Title:** Peer-to-Peer Streaming Peer Protocol (PPSPP)
- **RFC Publication Date:** July 2015
- Link to original errata report: [rfc-editor.org/errata/eid4880](https://www.rfc-editor.org/errata/eid4880)

```
Section 7.5 says:


   A peer MUST include the content integrity method used by a swarm.

   The code for this option is 3.  Defined values are listed in Table 4.



                   +--------+-------------------------+

                   | Method | Description             |

                   +--------+-------------------------+

                   | 0      | No integrity protection |

                   | 1      | Merkle Hash Tree        |

                   | 2      | Sign All                |

                   | 3      | Unified Merkle Tree     |

                   | 4-255  | Unassigned              |

                   +--------+-------------------------+



            Table 4: PPSPP Content Integrity Protection Methods

// state how to fix the above text here

```

## Issue description

This section includes a contradiction between the textual requirement of integrity protection methods and table 4. This inconsistency would lead to implementations allowing for undefined behavior.
