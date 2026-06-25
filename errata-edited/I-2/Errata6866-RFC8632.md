# Errata 6866 - RFC 8632

- **RFC Title:** A YANG Data Model for Alarm Management
- **RFC Publication Date:** September 2019

```
Section 6 says:


      container older-than {

        presence "Age specification";

        description

          "Matches the 'last-status-change' leaf in the alarm.";

        choice age-spec {

// state how to fix the above text here

Notes:


See also https://mailarchive.ietf.org/arch/msg/ccamp/wmCgk0DQq0lG6S_e59W-MKW8EOQ/
```

## Issue description

The original text refers to a non-existent leaf. This inconsistency would affect implementations that try to use this container to filter alarms.
