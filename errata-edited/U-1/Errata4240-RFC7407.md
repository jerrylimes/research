# Errata 4240 - RFC 7407

- **RFC Title:** A YANG Data Model for SNMP Configuration
- **RFC Publication Date:** December 2014

```
Section 4.8 says:


     augment /snmp:snmp/snmp:target {

       when "snmp:v1 or snmp:v2c";

// state how to fix the above text here

```

## Issue description

The original text includes a "when" expression that refers to non-existent nodes. This inconsistency makes the augment statement invalid and will lead to incorrect configuration processing.

**For this example, the correct fix has been provided to you as a guide to how to correctly disambiguate the erroneous text.**

## Correct fix

```
It should say:

     augment /snmp:snmp/snmp:target {
```
