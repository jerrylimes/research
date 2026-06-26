# Errata 7313 - RFC 8519

- **RFC Title:** YANG Data Model for Network Access Control Lists (ACLs)
- **RFC Publication Date:** March 2019

```
Section A.1 says:


   The following figure is the tree diagram of example-newco-acl.  In

   this example, /ietf-acl:acls/ietf-acl:acl/ietf-acl:aces/ietf-acl:ace/

   ietf-acl:matches are augmented with two new choices: protocol-

   payload-choice and metadata.  The protocol-payload-choice uses a

   grouping with an enumeration of all supported protocol values.

   Metadata matches apply to fields associated with the packet, that are

   not in the packet header, such as overall packet length.  In another

   example, /ietf-acl:acls/ietf-acl:acl/ietf-acl:aces/ietf-acl:ace/

   ietf-acl:actions are augmented with a new choice of actions.

// state how to fix the above text here

```

## Issue description

The original text uses a nonexistent prefix. This inconsistency affects the XPath expressions used for augmentation, making them invalid and impacting the implementation.
