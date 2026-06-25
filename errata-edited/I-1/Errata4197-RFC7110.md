# Errata 4197 - RFC 7110

- **RFC Title:** Return Path Specified Label Switched Path (LSP) Ping
- **RFC Publication Date:** January 2014

```
Section 4 says:


The Reply Path TLV contains one or more nested sub-TLVs that can be

used

// state how to fix the above text here

```

## Issue description

Section 4 of RFC 7110 provides an introductory description of the Reply Path TLV, but that description is inconsistent with the more detailed specification in Section 4.2. Implementations that rely solely on Section 4's description may incorrectly handle messages that are otherwise valid per Section 4.2.
