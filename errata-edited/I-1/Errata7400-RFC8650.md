# Errata 7400 - RFC 8650

- **RFC Title:** Dynamic Subscription to YANG Events and Datastores over RESTCONF
- **RFC Publication Date:** November 2019

```
Section Appendix A.3 says:


   POST /restconf/operations

        /ietf-subscribed-notifications:establish-subscription

   {

      "ietf-subscribed-notifications:input": {

         "stream": "NETCONF",

         "stream-xpath-filter":

           "/ietf-vrrp:vrrp-protocol-error-event[

             protocol-error-reason='checksum-error']/",

      }

   }



       Figure 16: Establishing a Subscription Error Reason via XPath



...



   POST /restconf/operations

        /ietf-subscribed-notifications:modify-subscription

   {

      "ietf-subscribed-notifications:input": {

         "stream": "NETCONF",

         "stream-subtree-filter": {

           "/ietf-vrrp:vrrp-protocol-error-event" : {}

         }

      }

   }

                Figure 17: Example "modify-subscription" RPC

// state how to fix the above text here

```

## Issue description

The errata report points out two stylistic issues that need to be corrected in the JSON figures provided in Appendix A.3 of RFC 8650 according to RFC9112's CRLF requirement.
