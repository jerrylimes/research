# Errata 7336 - RFC 9115

- **RFC Title:** An Automatic Certificate Management Environment (ACME) Profile for Generating Delegated Certificates
- **RFC Publication Date:** September 2021

```
Section Appendix A says:


   oid = text .regexp "([0-2])((\.0)|(\.[1-9][0-9]*))*"

// state how to fix the above text here

```

## Issue description

The original regular expression for the oid parameter incorrectly uses single backslashes to escape the period character in the CDDL string.
