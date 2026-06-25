# Errata 5756 - RFC 8040

- **RFC Title:** RESTCONF Protocol
- **RFC Publication Date:** January 2017

```
Section 8 says:


  module ietf-system {

    leaf system-reset {

      type empty;

    }

  }

// state how to fix the above text here

```

## Issue description

The example YANG module in Section 8 uses the wrong name that is inconsistent with the name "system-restart" discussed and referenced earlier for an RPC operation in the RFC from RFC 7317.  This inconsistency could lead to confusion and incorrect implementation of the system restart functionality.
