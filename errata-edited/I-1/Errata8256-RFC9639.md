# Errata 8256 - RFC 9639

- **RFC Title:** Free Lossless Audio Codec (FLAC)
- **RFC Publication Date:** December 2024

```
Section 8.2 says:


   SSAAAAAASSBBBBBBSSCCCCCC

   ^   ^   ^   ^   ^   ^

   |   |   |   |   |  Bits of 2nd sample of 1st channel

   |   |   |   |  Sign extension bits of 2nd sample of 2nd channel

   |   |   |  Bits of 1st sample of 2nd channel

   |   |  Sign extension bits of 1st sample of 2nd channel

   |  Bits of 1st sample of 1st channel

   Sign extension bits of 1st sample of 1st channel

// state how to fix the above text here

```

## Explanation

The diagram contains a label with an incorrect channel. The correction uses the correct channel for the sign extension bits, aligning the diagram with the described interleaving and sign-extension method.
