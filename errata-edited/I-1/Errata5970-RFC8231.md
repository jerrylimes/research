# Errata 5970 - RFC 8231

- **RFC Title:** Path Computation Element Communication Protocol (PCEP) Extensions for Stateful PCE
- **RFC Publication Date:** September 2017
- Link to original errata report: [rfc-editor.org/errata/eid5970](https://www.rfc-editor.org/errata/eid5970)

```
Section 8.5 says:


19       Invalid Operation



                Error-value

                1:   Attempted LSP Update Request for a non-delegated

                     LSP.  The PCEP-ERROR object is followed by the LSP

                     object that identifies the LSP.

// state how to fix the above text here

```

## Issue description

The original text contains irrelevant information. This inconsistency affects the interpretation and implementation of error reporting in stateful PCE.
