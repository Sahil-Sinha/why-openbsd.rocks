---
title: "Swap Encryption"
---

To protect sensitive information such as passwords from leaking to disk,
where they can persist for many years, OpenBSD supports encryption of the
swap partition. This is enabled by default!

```
sysctl vm.swapencrypt.enable=1
```

Details:

* [sysctl(2) - OpenBSD manual pages](https://man.openbsd.org/sysctl.2#VM_SWAPENCRYPT_2)
