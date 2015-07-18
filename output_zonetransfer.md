# Scanning for Zone Transfer on owasp.org #

```

*$ ./knock.py -zt owasp.org*

Knock v1.4.4b by Gianni 'guelfoweb' Amato ( http://knock.googlecode.com )

[+] Testing domain
www.owasp.org            216.48.3.18
[+] Dns resolving
Domain name               Ip address              Name server
No address associated with hostname owasp.org
[+] Getting NS records for owasp.org

Found name server: ns1.secure.net.
Found name server: ns2.secure.net.

[+] Trying a zone transfer for owasp.org from name server ns1.secure.net.

@	86400 IN SOA ns1.secure.net. hostmaster.secure.net. 2007080389 86400 7200 2592000 86400

@	86400 IN A 216.48.3.18

@	86400 IN NS ns2.secure.net.
86400 IN NS ns1.secure.net.

@	86400 IN MX 30 ASPMX5.GOOGLEMAIL.COM.
86400 IN MX 10 ASPMX.L.GOOGLE.COM.
86400 IN MX 20 ALT1.ASPMX.L.GOOGLE.COM.
86400 IN MX 20 ALT2.ASPMX.L.GOOGLE.COM.
86400 IN MX 30 ASPMX2.GOOGLEMAIL.COM.
86400 IN MX 30 ASPMX3.GOOGLEMAIL.COM.
86400 IN MX 30 ASPMX4.GOOGLEMAIL.COM.

@	86400 IN TXT "google-site-verification=I9qx_X9EKlR_rfceG25-iXHBXJ-vLrmeNbkEdy182iI"
86400 IN TXT "v=spf1 include:aspmx.googlemail.com ~all"

es	86400 IN A 216.48.3.18

pythonsecurity	86400 IN CNAME @

localhost	86400 IN A 127.0.0.1

ml1lists	86400 IN A 216.48.3.30

ads	86400 IN A 216.48.3.26

mail	86400 IN CNAME ghs.GOOGLE.COM.

*	86400 IN CNAME @

sl	86400 IN CNAME ghs.GOOGLE.COM.

austin	86400 IN CNAME @

www	86400 IN CNAME @

groups	86400 IN CNAME ghs.GOOGLE.COM.

docs	86400 IN CNAME ghs.GOOGLE.COM.

google6912a08c3a8cdf0b	86400 IN CNAME GOOGLE.COM.

forums	86400 IN A 216.48.3.19

lists	86400 IN A 216.48.3.22

lists	86400 IN MX 10 ml1lists

calendar	86400 IN CNAME ghs.GOOGLE.COM.

jobs	86400 IN CNAME @

[+] Trying a zone transfer for owasp.org from name server ns2.secure.net.

@	86400 IN SOA ns1.secure.net. hostmaster.secure.net. 2007080389 86400 7200 2592000 86400

@	86400 IN A 216.48.3.18

@	86400 IN NS ns1.secure.net.
86400 IN NS ns2.secure.net.

@	86400 IN MX 30 ASPMX4.GOOGLEMAIL.COM.
86400 IN MX 30 ASPMX5.GOOGLEMAIL.COM.
86400 IN MX 10 ASPMX.L.GOOGLE.COM.
86400 IN MX 20 ALT1.ASPMX.L.GOOGLE.COM.
86400 IN MX 20 ALT2.ASPMX.L.GOOGLE.COM.
86400 IN MX 30 ASPMX2.GOOGLEMAIL.COM.
86400 IN MX 30 ASPMX3.GOOGLEMAIL.COM.

@	86400 IN TXT "google-site-verification=I9qx_X9EKlR_rfceG25-iXHBXJ-vLrmeNbkEdy182iI"
86400 IN TXT "v=spf1 include:aspmx.googlemail.com ~all"

es	86400 IN A 216.48.3.18

pythonsecurity	86400 IN CNAME @

localhost	86400 IN A 127.0.0.1

ml1lists	86400 IN A 216.48.3.30

ads	86400 IN A 216.48.3.26

mail	86400 IN CNAME ghs.GOOGLE.COM.

*	86400 IN CNAME @

sl	86400 IN CNAME ghs.GOOGLE.COM.

austin	86400 IN CNAME @

www	86400 IN CNAME @

groups	86400 IN CNAME ghs.GOOGLE.COM.

docs	86400 IN CNAME ghs.GOOGLE.COM.

google6912a08c3a8cdf0b	86400 IN CNAME GOOGLE.COM.

forums	86400 IN A 216.48.3.19

lists	86400 IN A 216.48.3.22

lists	86400 IN MX 10 ml1lists

calendar	86400 IN CNAME ghs.GOOGLE.COM.

jobs	86400 IN CNAME @```