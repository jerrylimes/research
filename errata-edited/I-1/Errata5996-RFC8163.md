# Errata 5996 - RFC 8163

- **RFC Title:** Transmission of IPv6 over Master-Slave/Token-Passing (MS/TP) Networks
- **RFC Publication Date:** May 2017
- Link to original errata report: [rfc-editor.org/errata/eid5996](https://www.rfc-editor.org/errata/eid5996)

```
Section Appendix B. says:


       /*

        * Sanity check the encoding to prevent the while() loop below

        * from overrunning the output buffer.

        */

       if (read_index + code > length)

         return 0;

// state how to fix the above text here

```

## Explanation

The original code does not accommodate an edge case in COBS encoding. This inconsistency would lead to implementations failing to detect errors in COBS encoded data.
