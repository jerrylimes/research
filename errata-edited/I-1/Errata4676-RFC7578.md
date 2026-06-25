# Errata 4676 - RFC 7578

- **RFC Title:** Returning Values from Forms: multipart/form-data
- **RFC Publication Date:** July 2015

```
Section 4.6. says:


       --AaB03x

       content-disposition: form-data; name="_charset_"



       iso-8859-1

       --AaB03x--

       content-disposition: form-data; name="field1"



       ...text encoded in iso-8859-1 ...

       AaB03x--

// state how to fix the above text here

Notes:

Boundary hyphens were misplaced, I think.
```

## Issue description

The multipart/form-data example in Section 4.6 of RFC 7578 contains boundary delimiters that are not correctly formed, making the example non-conformant with the multipart format. Implementations using this example as a reference could produce invalid messages.
