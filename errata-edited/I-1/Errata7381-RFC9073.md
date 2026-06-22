# Errata 7381 - RFC 9073

- **RFC Title:** Event Publishing Extensions to iCalendar
- **RFC Publication Date:** August 2021
- Link to original errata report: [rfc-editor.org/errata/eid7381](https://www.rfc-editor.org/errata/eid7381)

```
Section 7.2 says:


   Format Definition:  This component is defined by the following

      notation:



      locationc    = "BEGIN" ":" "VLOCATION" CRLF

                     locprop

                     "END" ":" "VLOCATION" CRLF



      locprop      = *(

                     ;

                     ; The following are REQUIRED

                     ; but MUST NOT occur more than once.

                     ;

                     uid /

                     ;

                     ; The following are OPTIONAL

                     ; but MUST NOT occur more than once.

                     ;

                     description / geo / loctype / name

                     ;

                     ; The following are OPTIONAL

                     ; and MAY occur more than once.

                     ;

                     sdataprop / iana-prop

                  )

// state how to fix the above text here

```

## Issue description

The original specification is missing a property from the list of allowed properties in the "locprop" definition, which is inconsistent with the example provided in RFC 9074 and the general allowance for URL properties in iCalendar.
