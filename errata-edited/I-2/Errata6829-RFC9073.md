# Errata 6829 - RFC 9073

- **RFC Title:** Event Publishing Extensions to iCalendar
- **RFC Publication Date:** August 2021

```
Section 7.1 says:


      partprop     = *(

                     ;

                     ; The following are REQUIRED

                     ; but MUST NOT occur more than once.

                     ;

                     participanttype / uid /

                     ;

                     ; The following are OPTIONAL

                     ; but MUST NOT occur more than once.

                     ;

                     calendaraddress / created / description / dtstamp /

                     geo / last-mod / priority / seq /

                     status / summary / url /

                     ;

                     ; The following are OPTIONAL

                     ; and MAY occur more than once.

                     ;

                     attach / categories / comment

                     contact / location / rstatus / related /

                     resources / strucloc / strucres /

                     styleddescription / sdataprop / iana-prop

                     ;

                     )

// state how to fix the above text here

```

## Issue description

The original specification includes properties that are not defined in the document. The removal of these undefined properties resolves the inconsistency.
