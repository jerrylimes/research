# Errata 7679 - RFC 7852

- **RFC Title:** Additional Data Related to an Emergency Call
- **RFC Publication Date:** July 2016

```
Section 6.1 says:


An example

   Call-Info header field for this would be:



   Call-Info:  https://www.example.com/23sedde3;

       purpose="EmergencyCallData.ProviderInfo"

// state how to fix the above text here

```

## Issue description

The original example assigns a value of incorrect data type to an attribute. This inconsistency between the example and the specification of the attribute type affects the interpretation and correct implementation of the Call-Info header field.
