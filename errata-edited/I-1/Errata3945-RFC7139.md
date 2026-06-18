# Errata 3945 - RFC 7139

- **RFC Title:** GMPLS Signaling Extensions for Control of Evolving G.709 Optical Transport Networks
- **RFC Publication Date:** March 2014
- Link to original errata report: [rfc-editor.org/errata/eid3945](https://www.rfc-editor.org/errata/eid3945)

```
Section 7 says:


For the ingress node, a Path message with SE style SHOULD also be

sent for decreasing the ODUflex bandwidth.

// state how to fix the above text here

This change, that looks to be a change of substance, has been verified with the authors to be an editorial issue that was caused by not keeping the paragraphs in synch.
```

## Issue description

Section 7 states that Shared Explicit (SE) style is required when increasing ODUflex bandwidth. However, the reported text uses a less mandatory language when describing the corresponding behavior for decreasing ODUflex bandwidth. This creates an inconsistency between the requirements for increasing and decreasing bandwidth.

**For this example, the correct fix has been provided to you as a reference to the disambiguation process.**

## Correct fix
```
It should say:

For the ingress node, a Path message with SE style MUST also be

sent for decreasing the ODUflex bandwidth.
```
