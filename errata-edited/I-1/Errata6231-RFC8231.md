# Errata 6231 - RFC 8231

- **RFC Title:** Path Computation Element Communication Protocol (PCEP) Extensions for Stateful PCE
- **RFC Publication Date:** September 2017
- Link to original errata report: [rfc-editor.org/errata/eid6231](https://www.rfc-editor.org/errata/eid6231)

```
Section 8.5 says:


      20       LSP State Synchronization Error



                Error-value

                1:   A PCE indicates to a PCC that it cannot process (an

                     otherwise valid) LSP State Report.  The PCEP-ERROR

                     object is followed by the LSP object that

                     identifies the LSP.

// state how to fix the above text here

```

## Issue description

The original text contains irrelevant information. This inconsistency affects the interpretation and implementation of error reporting in stateful PCE.
