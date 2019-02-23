# git RPC failed

https://www.cnblogs.com/xiguapijiamuguanaicha/p/6508521.html

>error: RPC failed; curl 18 transfer closed with outstanding read data remaining 

>fatal: The remote end hung up unexpectedly 

>fatal: early EOF 

>fatal: index-pack failed

```shell
git config –-global http.postBuffer 524288000
```

```shell
git config –list
```

# git error: RPC failed; curl 56 LibreSSL SSL_read: SSL_ERROR_SYSCALL, errno 54

https://github.com/lanlin/notes/issues/41

```shell
git config http.postBuffer 524288000
git config https.postBuffer 524288000
```
