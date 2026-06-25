# Errata 7306 - RFC 9110

- **RFC Title:** HTTP Semantics
- **RFC Publication Date:** June 2022

```
Section 14.1.1 says:


  ranges-specifier = range-unit "=" range-set

  range-set        = 1#range-spec

  range-spec       = int-range

                   / suffix-range

                   / other-range

// state how to fix the above text here

```

## Explanation

The ABNF for ranges-specifier in Section 14.1.1 is inconsistent with the example provided in Section 14.1.2.
