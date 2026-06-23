# Errata 7833 - RFC 9483

- **RFC Title:** Lightweight Certificate Management Protocol (CMP) Profile
- **RFC Publication Date:** November 2023
- Link to original errata report: [rfc-editor.org/errata/eid7833](https://www.rfc-editor.org/errata/eid7833)

```
Section 4.1.6 says:


-- MUST be 0 for recipientInfo type PasswordRecipientInfo

// state how to fix the above text here

```

## Issue description

The original text specifies an incorrect value for the version number when using PasswordRecipientInfo. This inconsistency would lead to implementations generating incorrectly formatted CMP messages.
