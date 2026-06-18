# Errata 4197 - RFC 7110

- **RFC Title:** Return Path Specified Label Switched Path (LSP) Ping
- **RFC Publication Date:** January 2014
- Link to original errata report: [rfc-editor.org/errata/eid4197](https://www.rfc-editor.org/errata/eid4197)

```
Section 4 says:


The Reply Path TLV contains one or more nested sub-TLVs that can be

used

// state how to fix the above text here

```

## Issue description

The first paragraph of Section 4 contains an overview of the two new TLVs that the section later introduces. This paragraph does not accurately describe how many nested sub-TLVs can be used to carry the specified return path information, which is elaborated in Section 4.2. This impacts implementation because an implementation relying on Section 4's description would incorrectly reject valid messages with a certain number of sub-TLVs.
