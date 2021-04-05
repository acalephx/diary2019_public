```bash

# 全局设置代理
git config --global http.proxy socks5://127.0.0.1:1086
git config --global https.proxy socks5://127.0.0.1:1086

# 全局取消
git config --global --unset http.proxy socks5://127.0.0.1:1086
git config --global --unset https.proxy socks5://127.0.0.1:1086


#只对github.com代理
git config --global http.https://github.com.proxy socks5://127.0.0.1:1086

#取消代理
git config --global --unset http.https://github.com.proxy
```

## go proxy

```shell
export ALL_PROXY=socks5://127.0.0.1:1086
export ALL_PROXY=http://127.0.0.1:1087
go env -w GO111MODULE=on

```

```shell
go env -w GO111MODULE=on
go env -w GOPROXY=https://goproxy.cn,direct
```

```shell

go env -w GOPROXY=https://goproxy.cn,direct
go env -w GOSUMDB=sum.golang.google.cn

```


https://www.jianshu.com/p/205aff65954a

.zshrc
```shell
alias setproxy="export ALL_PROXY=socks5://127.0.0.1:1086"
alias setproxyhttp="export ALL_PROXY=http://127.0.0.1:1087"
alias unsetproxy="unset ALL_PROXY"

```
```shell
alias agent="git config --global http.proxy socks5://127.0.0.1:1086;git config --global https.proxy socks5://127.0.0.1:1086;git config --global http.sslVerify false"
alias unagent="git config --global --unset http.proxy;git config --global --unset https.proxy"
```
or
```shell
alias agent="git config --global http.proxy http://127.0.0.1:1087;git config --global https.proxy http://127.0.0.1:1087;git config --global http.sslVerify false"
alias unagent="git config --global --unset http.proxy;git config --global --unset https.proxy"

```
