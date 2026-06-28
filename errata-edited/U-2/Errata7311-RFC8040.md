# Errata 7311 - RFC 8040

- **RFC Title:** RESTCONF Protocol
- **RFC Publication Date:** January 2017

```
Section 7 says:


              +-------------------------+------------------+

              | error-tag               | status code      |

              +-------------------------+------------------+

(...)

              | unknown-attribute       | 400              |

              |                         |                  |

              | bad-element             | 400              |

(...)

// state how to fix the above text here

```

## Issue description

The table in Section 7 mapping error tags to HTTP status codes is missing an error-tag. This omission is inconsistent with the inclusion of other error tags, including an obsolete one.
