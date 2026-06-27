# Errata 4439 - RFC 7240

- **RFC Title:** Prefer Header for HTTP
- **RFC Publication Date:** June 2014

```
Section 2 says:


     preference = token [ BWS "=" BWS word ]

                  *( OWS ";" [ OWS parameter ] )

     parameter  = token [ BWS "=" BWS word ]

// state how to fix the above text here

```

## Issue description

The original specification uses an undefined term "word" in the definition of `preference` and `parameter`, rendering the syntax incomplete and making it impossible to unambiguously implement support for the Prefer header.
