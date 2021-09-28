# Apache 2.4.49 - Proxy via mod_rewrite and socket file broken

Steps to reproduce:

```sh
docker-compose up
```

Browse to http://localhost:1234/ notice error 5xx, change apache version in docker file to 2.4.48 and it all works fine.
