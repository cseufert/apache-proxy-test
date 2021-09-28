# Apache 2.4.49 - Proxy via mod_rewrite and socket file broken

Steps to reproduce:

1. Start Docker Container

```sh
docker-compose up
```

2. Browse to older apache version

Browse to http://localhost:8048/ and everything works (this is hosted with apache 2.4.48)

3. Browse to latest apache version

Browse to http://localhost:8049/ notice error, this can also result in path too long if path to socket is bit longer
