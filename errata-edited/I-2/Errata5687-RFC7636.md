# Errata 5687 - RFC 7636

- **RFC Title:** Proof Key for Code Exchange by OAuth Public Clients
- **RFC Publication Date:** September 2015

```
Section 5 says:


Server implementations of this specification MAY accept OAuth2.0

clients that do not implement this extension.  If the "code_verifier"

is not received from the client in the Authorization Request, servers

supporting backwards compatibility revert to the OAuth 2.0 [RFC6749]

protocol without this extension.



As the OAuth 2.0 [RFC6749] server responses are unchanged by this

specification, client implementations of this specification do not

need to know if the server has implemented this specification or not

and SHOULD send the additional parameters as defined in Section 4 to

all servers.

// state how to fix the above text here

```

## Issue description

The original text does not correctly identify the parameter that may be absent in an authorization request. This inconsistency affects implementations that need to correctly handle the absence of the code_challenge parameter.
