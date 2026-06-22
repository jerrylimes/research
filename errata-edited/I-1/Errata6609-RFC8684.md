# Errata 6609 - RFC 8684

- **RFC Title:** TCP Extensions for Multipath Operation with Multiple Addresses
- **RFC Publication Date:** March 2020
- Link to original errata report: [rfc-editor.org/errata/eid6609](https://www.rfc-editor.org/errata/eid6609)

```
Section B.3 says:


   initiator                                                    listener

       |                                                           |

       |    S  0(20) <MP_CAPABLE>, <TFO cookie>                    |

       | --------------------------------------------------------> |

       |                                                           |

       |    S. 0(0) ack 21 <MP_CAPABLE>                            |

       | <-------------------------------------------------------- |

       |                                                           |

       |    .  1(100) ack 21 <DSS ack=1 seq=1 ssn=1 dlen=100>      |

       | <-------------------------------------------------------- |

       |                                                           |

       |    .  21(0) ack 1 <MP_CAPABLE>                            |

       | --------------------------------------------------------> |

       |                                                           |

       |    .  21(20) ack 101 <DSS ack=101 seq=1 ssn=1 dlen=20>    |

       | --------------------------------------------------------> |

       |                                                           |



                    Figure 19: The Listener Supports TFO

// state how to fix the above text here

```

## Issue description

The example in Figure 19 shows the listener sending a DSS packet containing incorrect data.
