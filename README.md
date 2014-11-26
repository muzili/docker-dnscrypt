docker-dnscrypt
=================

[DNSCrypt][dnscrypt] for Docker.
[dnscrypt]: http://dnscrypt.org/

## Image Creation

This example creates the image with the tag `muzili/dnscrypt`, but you can change this to use your own username.

```
$ docker build -t="muzili/dnscrypt" .
```

Alternately, you can run the following if you have *make* installed...

```
$ make
```

You can also specify custom variables by change the Makefile.

You can run it by the following command...

```
$ docker run --name dnscrypt -d -p 53:53 -p 53:53/udp muzili/dnscrypt
```


## Environment variables

 - `RESOLVER_NAME`: Resolver name of dnscrypt. Default: `opendns`
