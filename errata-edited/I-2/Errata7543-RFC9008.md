# Errata 7543 - RFC 9008

- **RFC Title:** Using RPI Option Type, Routing Header for Source Routes, and IPv6-in-IPv6 Encapsulation in the RPL Data Plane
- **RFC Publication Date:** April 2021

```
Section 6 says:


As the Rank information in the RPI artifact is changed at each hop, it

will typically be zero when it arrives at the DODAG root.

// state how to fix the above text here

```

## Issue description

The original text contradicts the typical case in reality. This inconsistency could lead to misinterpretations of the RPI artifact.
