# Errata 5274 - RFC 7950

- **RFC Title:** The YANG 1.1 Data Modeling Language
- **RFC Publication Date:** August 2016
- Link to original errata report: [rfc-editor.org/errata/eid5274](https://www.rfc-editor.org/errata/eid5274)

```
Section 7.16.3 says:


   A corresponding XML instance example of the complete notification:



     <notification

       xmlns="urn:ietf:params:xml:ns:netconf:notification:1.0">

       <eventTime>2008-07-08T00:01:00Z</eventTime>

       <event xmlns="urn:example:event">

         <event-class>fault</event-class>

         <reporting-entity>

           /ex:interface[ex:name='Ethernet0']

         </reporting-entity>

         <severity>major</severity>

       </event>

     </notification>

// state how to fix the above text here

```

## Issue description

The original XML example is invalid because it has a missing namespace. This inconsistency would cause issues for implementations that validate the XML instance against the YANG module.
