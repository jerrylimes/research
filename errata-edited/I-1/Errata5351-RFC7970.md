# Errata 5351 - RFC 7970

- **RFC Title:** The Incident Object Description Exchange Format Version 2
- **RFC Publication Date:** November 2016

```
Section 2.16 says:


The attributes of the iodef:ExtensionType type are:



   name

      Optional.  STRING.  A free-form name of the field or data element.



   dtype

      Required.  ENUM.  The data type of the element content.  The

      default value is "string".  These values are maintained in the

      "ExtensionType-dtype" IANA registry per Section 10.2.



      1.   boolean.  The element content is of type BOOLEAN.



      2.   byte.  The element content is of type BYTE.



      3.   bytes.  The element content is of type HEXBIN.



      4.   character.  The element content is of type CHARACTER.



      5.   date-time.  The element content is of type DATETIME.



      6.   ntpstamp.  Same as date-time.



      7.   integer.  The element content is of type INTEGER.



      8.   portlist.  The element content is of type PORTLIST.



      9.   real.  The element content is of type REAL.



      10.  string.  The element content is of type STRING.



      11.  file.  The element content is a base64-encoded binary file

           encoded as a BYTE[] type.



      12.  path.  The element content is a file-system path encoded as a

           STRING type.



      13.  frame.  The element content is a Layer 2 frame encoded as a

           HEXBIN type.



      14.  packet.  The element content is a Layer 3 packet encoded as a

           HEXBIN type.



      15.  ipv4-packet.  The element content is an IPv4 packet encoded

           as a HEXBIN type.



      16.  ipv6-packet.  The element content is an IPv6 packet encoded

           as a HEXBIN type.



      17.  url.  The element content is of type URL.



      18.  csv.  The element content is a comma-separated value (CSV)

           list per Section 2 of [RFC4180] encoded as a STRING type.



      19.  winreg.  The element content is a Microsoft Windows registry

           key encoded as a STRING type.



      20.  xml.  The element content is XML.  See Section 5.2.



      21.  ext-value.  A value used to indicate that this attribute is

           extended and the actual value is provided using the

           corresponding ext-* attribute.  See Section 5.1.1.

// state how to fix the above text here

```

## Issue description

Dtype descriptions that use multiple bytes are not using the correct data type in Section 2.16. This inconsistency could lead to implementations incorrectly interpreting the data types.
