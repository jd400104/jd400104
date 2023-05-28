
Build

```
./build.sh -O ../obj -T ../tools -U -u -j8 distribution 2>&1 > ~/build.distribution.log && \
./build.sh -O ../obj -T ../tools -U -u -j8 kernel=GENERIC64 2>&1 > ~/build.kernel.log && \
./build.sh -O ../obj -T ../tools -U install=/
date
```

Install

```
 /usr/sbin/postinstall -s /home/test/cvs/src check
 /usr/sbin/postinstall -s /home/test/cvs/src fix
 /usr/sbin/etcupdate -s /home/test/cvs/src
```

[32.4.3. Fetching the NetBSD-current development branch](http://netbsd.org/docs/guide/en/chap-fetch.html#chap-fetch-cvs-netbsd-current)


[Chapter 35, Updating an existing system from sources](http://netbsd.org/docs/guide/en/chap-updating.html)
