# Errata 6873 - RFC 8984

- **RFC Title:** JSCalendar: A JSON Representation of Calendar Data
- **RFC Publication Date:** July 2021

```
Section 4.3.2. says:


Identifies the time zone of the main JSCalendar object, of which this

JSCalendar object is a recurrence instance.  This property MUST be

set if the "recurrenceId" property is set.  It MUST NOT be set if the

"recurrenceId" property is not set.

// state how to fix the above text here

```

## Issue description

The original description adds a restriction that doesn't take the possibility of a recurrence instance in floating time into account.
