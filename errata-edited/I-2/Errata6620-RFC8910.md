# Errata 6620 - RFC 8910

- **RFC Title:** Captive-Portal Identification in DHCP and Router Advertisements (RAs)
- **RFC Publication Date:** September 2020

```
Section 2 says:


   A captive portal MAY do content negotiation (Section 3.4 of

   [RFC7231]) and attempt to redirect clients querying without an

   explicit indication of support for the captive portal API content

   type (i.e., without application/capport+json listed explicitly

   anywhere within an Accept header field as described in Section 5.3 of

   [RFC7231]).  In so doing, the captive portal SHOULD redirect the

   client to the value associated with the "user-portal-url" API key.

   When performing such content negotiation (Section 3.4 of [RFC7231]),

   implementors of captive portals need to keep in mind that such

   responses might be cached, and therefore SHOULD include an

   appropriate Vary header field (Section 7.1.4 of [RFC7231]) or set the

   Cache-Control header field in any responses to "private" or a more

   restrictive value such as "no-store" (Section 5.2.2.3 of [RFC7234]).

// state how to fix the above text here

```

## Issue description

The original text uses a content type that is inconsistent with RFC 8908 when explaining what "captive portal API content type" is.
