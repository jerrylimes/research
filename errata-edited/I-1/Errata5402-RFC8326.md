# Errata 5402 - RFC 8326

- **RFC Title:** Graceful BGP Session Shutdown
- **RFC Publication Date:** March 2018

```
Section C.2.2. says:


      4.  If, for any reason, RR3 processes the withdraw generated in

          step 3 before processing the update generated in step 2, RR3

          transiently suffers from unreachability for the affected

          prefix.

// state how to fix the above text here

```

## Explanation

The original text refers to the incorrect Route Reflector (RR).  This inconsistency affects the accuracy of the example and could lead to misinterpretations of the graceful BGP session shutdown procedure.
