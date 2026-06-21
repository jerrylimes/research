# Errata 5545 - RFC 8152

- **RFC Title:** CBOR Object Signing and Encryption (COSE)
- **RFC Publication Date:** July 2017
- Link to original errata report: [rfc-editor.org/errata/eid5545](https://www.rfc-editor.org/errata/eid5545)

```
Section 7.1 says:


   +---------+-------+----------------+------------+-------------------+

   | Name    | Label | CBOR Type      | Value      | Description       |

   |         |       |                | Registry   |                   |

   +---------+-------+----------------+------------+-------------------+

   | kty     | 1     | tstr / int     | COSE Key   | Identification of |

   |         |       |                | Common     | the key type      |

   |         |       |                | Parameters |                   |

   |         |       |                |            |                   |

   | kid     | 2     | bstr           |            | Key               |

   |         |       |                |            | identification    |

   |         |       |                |            | value -- match to |

   |         |       |                |            | kid in message    |

   |         |       |                |            |                   |

   | alg     | 3     | tstr / int     | COSE       | Key usage         |

   |         |       |                | Algorithms | restriction to    |

   |         |       |                |            | this algorithm    |

   |         |       |                |            |                   |

   | key_ops | 4     | [+ (tstr/int)] |            | Restrict set of   |

   |         |       |                |            | permissible       |

   |         |       |                |            | operations        |

   |         |       |                |            |                   |

   | Base IV | 5     | bstr           |            | Base IV to be     |

   |         |       |                |            | xor-ed with       |

   |         |       |                |            | Partial IVs       |

   +---------+-------+----------------+------------+-------------------+



                          Table 3: Key Map Labels

// state how to fix the above text here

```

## Issue description

The original table uses an incorrect term to describe the value registry for the kty parameter that is not consistent with the text following it.
