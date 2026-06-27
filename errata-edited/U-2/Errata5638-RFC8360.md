# Errata 5638 - RFC 8360

- **RFC Title:** Resource Public Key Infrastructure (RPKI) Validation Reconsidered
- **RFC Publication Date:** April 2018

```
Section 4.2.4.4 says:


   7.  Compute the VRS-IP and VRS-AS set values as indicated below:



       *  If the IP Address Delegation extension is present in

          certificate x and x=1, set the VRS-IP to the resources found

          in this extension.



       *  If the IP Address Delegation extension (...)



       *  If the IP Address Delegation extension (...)



       *  If the IP Address Delegation extension is present in

          certificate x and x=1, set the VRS-IP to the resources found

          in this extension.



       *  If the AS Identifier Delegation extension (...)



       *  If the AS Identifier Delegation extension (...)

// state how to fix the above text here

```

## Issue description

The original text contains duplicate bullet points for handling the IP Address Delegation extension.
