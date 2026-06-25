# Errata 5255 - RFC 8040

- **RFC Title:** RESTCONF Protocol
- **RFC Publication Date:** January 2017

```
Section 3.5.3. says:


If there are multiple key leaf values, the path 

segment is constructed by having the list name, 

followed by the value of each leaf identified 

in the "key" statement, encoded in the order

specified in the YANG "key" statement.  Each key 

leaf value except the last one is followed by 

a comma character.

// state how to fix the above text here

```

## Issue description

The description of key value encoding in Section 3.5.3 does not accurately reflect the example path segments provided in that section. This inconsistency could lead to incorrect implementation of key value encoding in RESTCONF clients and servers.
