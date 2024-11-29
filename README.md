# Apache 2.4.61 - Proxy via mod_rewrite and socket file regression

Steps to reproduce:

1. Start Docker Container

```sh
docker-compose up
```

2. Browse to 2.4.61 apache version

Browse to http://localhost:8061/ and everything works (this is hosted with apache 2.4.48)

3. Browse to 2.4.62 apache version

Browse to http://localhost:8062/ Errors out trying to access socket

Log:

```
[proxy:warn] [pid 8:tid 12] [client 172.21.0.1:42238] AH01144: No protocol handler was valid for the URL /index.html (scheme 'unix'). If you are using a DSO version of mod_proxy, make sure the proxy submodules are included in the configuration using LoadModule.

```
