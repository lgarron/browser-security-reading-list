# Browser Security Reading List and References

There are a lot of lists about cryptography and security.
This is my personal list, focused on documents that are relevant to my work on the [Chrome security UX team](https://www.chromium.org/Home/chromium-security/enamel).

It simultaneously lets me document the kinds of things one needs to know to work in my area, and gives me an easy way to find references I may need in the future (either for myself, or to give to others).

Expect it to be incomplete at all times.

## Origin

The "origin" is a (scheme, host, tuple), e.g. (https, www.google.com, 443). It is the most important concept for site isolation on the web.

- [RFC 6454](https://tools.ietf.org/html/rfc6454): The Origin Concept (Adam Barth, 2011)
- [Same-origin policy at Wikipedia](https://en.wikipedia.org/wiki/Same-origin_policy)
- Suborigin proposal: [Chromium page](http://www.chromium.org/developers/design-documents/per-page-suborigins) and [blog post](http://blog.joelweinberger.us/2013/08/suborigins-for-privilege-separation-in.html) (Joel Weinberger, 2014)

## HSTS

HTTP Strict Transport Security is a mechanism for a server to tell a browser "only connect to me over HTTPS in the future". It can be sent via the `Strict-Transport-Security` header and/or be built into browsers for specific sites.

- [RFC 6797](https://tools.ietf.org/html/rfc6797): HTTP Strict Transport Security (Hodges, Jackson, and Barth, 2012)
- [HSTS at Wikipedia](https://en.wikipedia.org/wiki/HTTP_Strict_Transport_Security)
- [chromium.org/hsts](https://www.chromium.org/hsts): Chromium info, link to preload list and submission page.
- [Upgrading HTTPS in Mid-Air](http://www.internetsociety.org/sites/default/files/01_4_0.pdf): An Empirical Study of Strict Transport Security and Key Pinning (Michael Kranch and Joseph Bonneau, 2015)

## TLS Deployment

- [Bulletproof SSL and TLS](https://www.feistyduck.com/books/bulletproof-ssl-and-tls/) book (Ivan Ristić, 2014)
- [Why Eve and Mallory (Also) Love Webmasters](http://dl.acm.org/citation.cfm?id=2590341): A Study on the Root Causes of SSL Misconfigurations (Fahl, Acar, Perl, Smith, 2014)

## SSL/TLS Interstitials

- [Improving SSL Warnings](https://adrifelt.github.io/sslinterstitial-chi.pdf): Comprehension and Adherence (Felt, Ainslie, Reeder, Consolvo, Thyagaraja, Bettes, Harris, Grimes, 2015)
