---
title: "pf(4)"
---

`pf` is OpenBSD's very own firewall, since 3.0. It is simple and feature-rich
and its configuration files are easy to read.  It supports the use of variables,
lists and tables.

```
tcpin = "{ http, https, ssh }"

block in all
pass out quick on $extif from any to any
pass in on $extif proto tcp from any to any port $tcpin
```

In fact, `pf` was often one of the top selling points for OpenBSD and many
commercial firewall appliances are based on it.

Details:

* [OpenBSD PF: User’s Guide](https://www.openbsd.org/faq/pf/)
* [pf.conf(5) - OpenBSD manual pages](https://man.openbsd.org/pf.conf.5)
* [pf(4) - OpenBSD manual pages](https://man.openbsd.org/pf)
* [OpenBSD 3.0](https://www.openbsd.org/30.html)
* [pf (firewall) - Wikipedia](https://en.wikipedia.org/wiki/PF_(firewall))
