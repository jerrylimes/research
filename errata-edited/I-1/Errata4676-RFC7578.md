# Errata 4676 - RFC 7578

- **RFC Title:** Returning Values from Forms: multipart/form-data
- **RFC Publication Date:** July 2015
- Link to original errata report: [rfc-editor.org/errata/eid4676](https://www.rfc-editor.org/errata/eid4676)

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

## Explanation

The original example incorrectly places boundary hyphens. This inconsistency could lead to implementations incorrectly parsing or generating multipart/form-data messages.
