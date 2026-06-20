# Errata 4874 - RFC 7181

- **RFC Title:** The Optimized Link State Routing Protocol Version 2
- **RFC Publication Date:** April 2014
- Link to original errata report: [rfc-editor.org/errata/eid4874](https://www.rfc-editor.org/errata/eid4874)

```
Section 17.1 says:


   If the router changes its originator address, then:



   1.  If there is no Originator Tuple with:



       *  O_orig_addr = old originator address



       then create an Originator Tuple with:



       *  O_orig_addr := old originator address



       The Originator Tuple (existing or new) with:



       *  O_orig_addr = new originator address



       is then modified as follows:



       *  O_time := current time + O_HOLD_TIME

// state how to fix the above text here

```

## Issue description

The original description contradicts itself regarding the handling of Originator Tuples when the originator address changes. This inconsistency would lead to incorrect management of Originator Tuples, affecting the routing protocol's operation.
