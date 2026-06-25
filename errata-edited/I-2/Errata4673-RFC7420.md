# Errata 4673 - RFC 7420

- **RFC Title:** Path Computation Element Communication Protocol (PCEP) Management Information Base (MIB) Module
- **RFC Publication Date:** December 2014
- Link to original errata report: [rfc-editor.org/errata/eid4673](https://www.rfc-editor.org/errata/eid4673)

```
Section 4.1 says:


pcePcepSessState OBJECT-TYPE

       SYNTAX      INTEGER {

                      tcpPending(1),

                      openWait(2),

                      keepWait(3),

                      sessionUp(4)

                   }

       MAX-ACCESS  read-only

       STATUS      current

       DESCRIPTION

           "The current state of the session.



            The set of possible states excludes the idle state since

            entries do not exist in this table in the idle state."

       ::= { pcePcepSessEntry 3 }

// state how to fix the above text here

```

## Issue description

The original specification for `pcePcepSessState` is missing a state that the notification pcePcepSessDown requires. The claim made in the DESCRIPTION to support this omission is also incorrect.
