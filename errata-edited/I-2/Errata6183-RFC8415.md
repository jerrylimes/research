# Errata 6183 - RFC 8415

- **RFC Title:** Dynamic Host Configuration Protocol for IPv6 (DHCPv6)
- **RFC Publication Date:** November 2018

```
Section 18.3.8 says:


   After all the addresses have been processed, the server generates a

   Reply message by setting the "msg-type" field to REPLY and copying

   the transaction ID from the Decline message into the "transaction-id"

   field.  The client includes a Status Code option (see Section 21.13)

   with the value Success, a Server Identifier option (see Section 21.3)

   with the server's DUID, and a Client Identifier option (see

   Section 21.2) with the client's DUID

// state how to fix the above text here

```

## Issue description

The original text does not correctly state which entity has the options in the Reply message. This inconsistency would affect implementations that incorrectly handle option inclusion in the Reply message.
