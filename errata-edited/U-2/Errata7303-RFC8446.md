# Errata 7303 - RFC 8446

- **RFC Title:** The Transport Layer Security (TLS) Protocol Version 1.3
- **RFC Publication Date:** August 2018

```
Section 6.1 says:


This alert notifies the recipient that the sender will not send any more messages on this connection. 

// state how to fix the above text here

```

## Issue description

The original text does not specify the severity level for close_notify alerts, which may lead to interoperability issues between implementations that treat alerts with different severity levels differently.
