# Errata 6078 - RFC 7950

- **RFC Title:** The YANG 1.1 Data Modeling Language
- **RFC Publication Date:** August 2016
- Link to original errata report: [rfc-editor.org/errata/eid6078](https://www.rfc-editor.org/errata/eid6078)

```
Section 6.4. says:


   For example, consider the following definition:



     leaf lxiv {

       type decimal64 {

         fraction-digits 18;

       }

       must ". <= 10";

     }



   An instance of the "lxiv" leaf having the value of

   10.0000000000000001 will then successfully pass validation.

// state how to fix the above text here

```

## Explanation

The original example contradicts the specified constraints. This inconsistency would lead to implementations incorrectly validating the example.
