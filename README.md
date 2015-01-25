I am
====

Simple whois server implementation

Setup
=====

First, you need inetd

```
apt-get install openbsd-inetd
```

Next, append this line to your `/etc/inetd.conf`.

```
whois           stream  tcp6 nowait  nobody /opt/iam/iam
```

This assumes you've cloned this repo into /opt.

Finally, put some text in `/etc/iam.txt` and reload the inetd.

License
-------

GPLv3
