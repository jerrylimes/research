# Errata 7929 - RFC 9562

- **RFC Title:** Universally Unique IDentifiers (UUIDs)
- **RFC Publication Date:** May 2024
- Link to original errata report: [rfc-editor.org/errata/eid7929](https://www.rfc-editor.org/errata/eid7929)

```
Section B.2 says:


custom_c  62   0b00, 0x38a375d0df1fbf6

// state how to fix the above text here

```

## Explanation

The original example uses an incorrect value for the custom_c variant. This inconsistency would affect implementations that rely on the correct values for UUID variants.
