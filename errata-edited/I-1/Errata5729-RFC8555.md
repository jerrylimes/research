# Errata 5729 - RFC 8555

- **RFC Title:** Automatic Certificate Management Environment (ACME)
- **RFC Publication Date:** March 2019

```
Section 7.5.1 says:


The client indicates to the server that it is ready for the challenge

validation by sending an empty JSON body ("{}") carried in a POST

request to the challenge URL (not the authorization URL).

// statw how to fix the above text here

```

## Issue description

The description of the challenge validation process in Section 7.5.1 is inconsistent with the requirement for a JWS-signed response object as defined in Section 8. This inconsistency affects client implementation which must correctly construct and sign the JWS object for challenge validation.
