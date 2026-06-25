# Errata 3944 - RFC 7139

- **RFC Title:** GMPLS Signaling Extensions for Control of Evolving G.709 Optical Transport Networks
- **RFC Publication Date:** March 2014

```
Section 5.1 says:


      ODUk.ts       Minimum          Nominal          Maximum

      -----------------------------------------------------------

      ODU2.ts    1,249,384.632    1,249,409.620     1,249,434.608

      ODU3.ts    1,254,678.635    1,254,703.729     1,254,728.823

      ODU4.ts    1,301,683.217    1,301,709.251     1,301,735.285



              Table 1: Actual TS Bit Rate of ODUk (in Kbps)

// state how to fix the above text here

```

## Issue description

Table 1 contains a typo. This inconsistency could lead to implementation issues if an implementation is strictly following the incorrect table in the original text.
