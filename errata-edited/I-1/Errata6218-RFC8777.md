# Errata 6218 - RFC 8777

- **RFC Title:** DNS Reverse IP Automatic Multicast Tunneling (AMT) Discovery
- **RFC Publication Date:** April 2020
- Link to original errata report: [rfc-editor.org/errata/eid6218](https://www.rfc-editor.org/errata/eid6218)

```
Section 4.3.2 says:


10   IN TYPE260  \# (

       18 ; length

       0a ; precedence=10

       02 ; D=0, relay type=2, an IPv6 address

       20010db800000000000000000000000f ) ; 2001:db8::15

10   IN TYPE260  \# (

       24 ; length

       80 ; precedence=128

       83 ; D=1, relay type=3, a wire-encoded domain name

       09616d7472656c617973076578616d706c6503636f6d ) ; domain name

// state how to fix the above text here

```

## Issue description

The two examples of Section 4.3.2 of RFC 8777 contains errors in encoding. Both errors are directly related to the correct implementation of the AMT discovery mechanism and will lead to incorrect interpretation of the data, therefore, the classification is INCONSISTENT.
