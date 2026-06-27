# Errata 4503 - RFC 7483

- **RFC Title:** JSON Responses for the Registration Data Access Protocol (RDAP)
- **RFC Publication Date:** March 2015

```
Section 5.2 and 5.3 says:


In Section 5.2:



"ldhName" : "ns1.xn--fo-5ja.example",

"unicodeName" : "ns1.foo.example",



In Section 5.3:



"ldhName" : "xn--fo-5ja.example",

"unicodeName" : "foo.example",



"ldhName" : "xn--fo-cka.example",

"unicodeName" : "foo.example"



"ldhName" : "xn--fo-fka.example",

"unicodeName" : "foo.example"



"ldhName": "xn--fo-8ja.example",

"unicodeName" : "foo.example"

// state how to fix the above text here

Notes:

The unicodeName examples in RFC 7483 are invalid per RFC 5890.
```

## Issue description

The `unicodeName` field examples in Sections 5.2 and 5.3 of RFC 7483 do not conform to the definition of Unicode names given in Section 3 and established by RFC 5890, creating an inconsistency between the stated requirements and the provided examples that could mislead implementers.
