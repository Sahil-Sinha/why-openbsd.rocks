---
title: "Chrooted webserver by default"
---

By default, HTTP daemons are chrooted in `/var/www`. As an OpenBSD
system administrator, you don't need to configure anything to have a 
secured webserver installation running.

This is also true for HTTP daemons from packages (`apache2`, `nginx`).

```
$ getent passwd www
www:*:67:67:HTTP Server:/var/www:/sbin/nologin
```

Details:

* [httpd.conf(5) - OpenBSD manual pages](https://man.openbsd.org/httpd.conf.5)
* [chroot(2) - OpenBSD manual pages](https://man.openbsd.org/man2/chroot.2)
* [chroot(8) - OpenBSD manual pages](https://man.openbsd.org/man2/chroot.8)
