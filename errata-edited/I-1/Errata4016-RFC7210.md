# Errata 4016 - RFC 7210

- **RFC Title:** Database of Long-Lived Symmetric Cryptographic Keys
- **RFC Publication Date:** April 2014
- Link to original errata report: [rfc-editor.org/errata/eid4016](https://www.rfc-editor.org/errata/eid4016)

```
Section 2 says:


      SendLifetimeStart

         The SendLifetimeStart field specifies the earliest date and

         time in Coordinated Universal Time (UTC) at which this key

         should be considered for use when sending traffic.  The format

         is YYYYMMDDHHSSZ, where four digits specify the year, two

         digits specify the month, two digits specify the day, two

         digits specify the hour, two digits specify the minute, and two

         digits specify the second.  The "Z" is included as a clear

         indication that the time is in UTC.



      SendLifeTimeEnd

         The SendLifeTimeEnd field specifies the latest date and time at

         which this key should be considered for use when sending

         traffic.  The format is the same as the SendLifetimeStart

         field.



      AcceptLifeTimeStart

         The AcceptLifeTimeStart field specifies the earliest date and

         time in Coordinated Universal Time (UTC) at which this key

         should be considered for use when processing received traffic.

         The format is YYYYMMDDHHSSZ, where four digits specify the

         year, two digits specify the month, two digits specify the day,

         two digits specify the hour, two digits specify the minute, and

         two digits specify the second.  The "Z" is included as a clear

         indication that the time is in UTC.


// state how to fix the above text here


```

## Issue description

The timestamp format strings used in the key lifetime fields of Section 2 do not match their accompanying prose descriptions, creating an ambiguity in how implementations should format and interpret these values.
