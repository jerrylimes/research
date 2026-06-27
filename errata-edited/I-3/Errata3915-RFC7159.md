# Errata 3915 - RFC 7159

- **RFC Title:** The JavaScript Object Notation (JSON) Data Interchange Format
- **RFC Publication Date:** March 2014

```
Section 12 says:


   Since JSON's syntax is borrowed from JavaScript, it is possible to

   use that language's "eval()" function to parse JSON texts.

// state how to fix the above text here

```

## Issue description

The original statement overestimates the "eval()" function's capability.

**For this example, the correct fix has been provided to you as a guide to how to correctly disambiguate the erroneous text.**

## Correct fix

```
It should say:

   Since JSON's syntax is borrowed from JavaScript, it is possible to

   use that language's "eval()" function to parse most (but not all)

   JSON texts.
```
