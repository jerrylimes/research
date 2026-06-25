# Errata 4935 - RFC 8080

- **RFC Title:** Edwards-Curve Digital Security Algorithm (EdDSA) for DNSSEC
- **RFC Publication Date:** February 2017

```
Section 6 says:


6.  Examples



6.1.  Ed25519 Examples



Private-key-format: v1.2

Algorithm: 15 (ED25519)

PrivateKey: ODIyNjAzODQ2MjgwODAxMjI2NDUxOTAyMDQxNDIyNjI=



example.com. 3600 IN DNSKEY 257 3 15 (

             l02Woi0iS8Aa25FQkUd9RMzZHJpBoRQwAQEX1SxZJA4= )



example.com. 3600 IN DS 3613 15 2 (

             3aa5ab37efce57f737fc1627013fee07bdf241bd10f3b1964ab55c78e79

             a304b )



example.com. 3600 IN MX 10 mail.example.com.



example.com. 3600 IN RRSIG MX 3 3600 (

             1440021600 1438207200 3613 example.com. (

             Edk+IB9KNNWg0HAjm7FazXyrd5m3Rk8zNZbvNpAcM+eysqcUOMIjWoevFkj

             H5GaMWeG96GUVZu6ECKOQmemHDg== )







Sury & Edmonds               Standards Track                    [Page 3]



RFC 8080                    EdDSA for DNSSEC               February 2017





Private-key-format: v1.2

Algorithm: 15 (ED25519)

PrivateKey: DSSF3o0s0f+ElWzj9E/Osxw8hLpk55chkmx0LYN5WiY=



example.com. 3600 IN DNSKEY 257 3 15 (

             zPnZ/QwEe7S8C5SPz2OfS5RR40ATk2/rYnE9xHIEijs= )



example.com. 3600 IN DS 35217 15 2 (

             401781b934e392de492ec77ae2e15d70f6575a1c0bc59c5275c04ebe80c

             6614c )



example.com. 3600 IN MX 10 mail.example.com.



example.com. 3600 IN RRSIG MX 3 3600 (

             1440021600 1438207200 35217 example.com. (

             5LL2obmzdqjWI+Xto5eP5adXt/T5tMhasWvwcyW4L3SzfcRawOle9bodhC+

             oip9ayUGjY9T/rL4rN3bOuESGDA== )



6.2.  Ed448 Examples



Private-key-format: v1.2

Algorithm: 16 (ED448)

PrivateKey: xZ+5Cgm463xugtkY5B0Jx6erFTXp13rYegst0qRtNsOYnaVpMx0Z/c5EiA9x

            8wWbDDct/U3FhYWA



example.com. 3600 IN DNSKEY 257 3 16 (

             3kgROaDjrh0H2iuixWBrc8g2EpBBLCdGzHmn+G2MpTPhpj/OiBVHHSfPodx

             1FYYUcJKm1MDpJtIA )



example.com. 3600 IN DS 9713 16 2 (

             6ccf18d5bc5d7fc2fceb1d59d17321402f2aa8d368048db93dd811f5cb2

             b19c7 )



example.com. 3600 IN MX 10 mail.example.com.



example.com. 3600 IN RRSIG MX 3 3600 (

             1440021600 1438207200 9713 example.com. (

             Nmc0rgGKpr3GKYXcB1JmqqS4NYwhmechvJTqVzt3jR+Qy/lSLFoIk1L+9e3

             9GPL+5tVzDPN3f9kAwiu8KCuPPjtl227ayaCZtRKZuJax7n9NuYlZJIusX0

             SOIOKBGzG+yWYtz1/jjbzl5GGkWvREUCUA )























Sury & Edmonds               Standards Track                    [Page 4]



RFC 8080                    EdDSA for DNSSEC               February 2017





Private-key-format: v1.2

Algorithm: 16 (ED448)

PrivateKey: WEykD3ht3MHkU8iH4uVOLz8JLwtRBSqiBoM6fF72+Mrp/u5gjxuB1DV6NnPO

            2BlZdz4hdSTkOdOA



example.com. 3600 IN DNSKEY 257 3 16 (

             kkreGWoccSDmUBGAe7+zsbG6ZAFQp+syPmYUurBRQc3tDjeMCJcVMRDmgcN

             Lp5HlHAMy12VoISsA )



example.com. 3600 IN DS 38353 16 2 (

             645ff078b3568f5852b70cb60e8e696cc77b75bfaaffc118cf79cbda1ba

             28af4 )



example.com. 3600 IN MX 10 mail.example.com.



example.com. 3600 IN RRSIG MX 3 3600 (

             1440021600 1438207200 38353 example.com. (

             +JjANio/LIzp7osmMYE5XD3H/YES8kXs5Vb9H8MjPS8OAGZMD37+LsCIcjg

             5ivt0d4Om/UaqETEAsJjaYe56CEQP5lhRWuD2ivBqE0zfwJTyp4WqvpULbp

             vaukswvv/WNEFxzEYQEIm9+xDlXj4pMAMA )

// state how to fix the above text here

```

## Issue description

Two issues are present in the original text. 1. The four examples are not correctly identifying algorithms. 2. The label counting implementation is incorrect in the RRSIG examples. Both directly impact the implementation and verification of signatures, causing the examples to be unimplementable as presented. This constitutes an inconsistency affecting critical implementation details.
