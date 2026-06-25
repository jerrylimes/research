# Errata 6922 - RFC 8466

- **RFC Title:** A YANG Data Model for Layer 2 Virtual Private Network (L2VPN) Service Delivery
- **RFC Publication Date:** October 2018

```
Section 5.5.2.1 says:


...

             <network-access-id>LA1</network-access-id>

                <service>

                  <svc-bandwidth>

                     <bandwidth>

                       <direction>input-bw</direction>

                        <type>bw-per-cos</type>

                         <cir>450000000</cir>

                         <cbs>20000000</cbs>

                         <eir>1000000000</eir>

                         <ebs>200000000</ebs>

                     </bandwidth>

                    </svc-bandwidth>

...

            <network-access-id>LA2</network-access-id>

                <service>

                  <svc-bandwidth>

                     <bandwidth>

                       <direction>input-bw</direction>

                        <type>bw-per-cos</type>

                         <cir>450000000</cir>

                         <cbs>20000000</cbs>

                         <eir>1000000000</eir>

                         <ebs>200000000</ebs>

// state how to fix the above text here

```

## Issue description

The original example is missing a parameter when the "type" attribute is set to "bw-per-cos". This inconsistency would lead to implementations incorrectly processing svc-bandwidth configurations.
