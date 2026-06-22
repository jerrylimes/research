# Errata 6258 - RFC 7950

- **RFC Title:** The YANG 1.1 Data Modeling Language
- **RFC Publication Date:** August 2016
- Link to original errata report: [rfc-editor.org/errata/eid6258](https://www.rfc-editor.org/errata/eid6258)

```
Section 5.6.5 says:


For example, with these modules:



     module a {

       yang-version 1.1;

       namespace "urn:example:a";

       prefix "a";



       import b {

         revision-date 2015-01-01;

       }

       import c;



       revision 2015-01-01;

// state how to fix the above text here

```

## Issue description

The original example is missing substatements within the "import" statements, violating the rules defined in Section 7.1.5. This inconsistency would affect implementations that rely on the example for guidance on the correct structure of import statements.
