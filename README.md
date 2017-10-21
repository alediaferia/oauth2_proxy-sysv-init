Oauth2 Proxy SysV Init File
---

A symple SysV init file for [Oauth2
Proxy](//github.com/bitly/oauth2_proxy)

**NOTE**: This script has only been tested on Amazon Linux

# How to use it
This init script expects the following paths to be present:

* `/usr/bin/oauth2_proxy`: the actual binary to launch
* `/etc/oauth2_proxy/oauth2_proxy.cfg`: the configuration file

Place this file under `/etc/init.d/`.

Run the following command to register it as a service:

```bash
$ chkconfig --add oauth2_proxy
```

Then start it using:

```bash
$ service oauth2_proxy start
```

