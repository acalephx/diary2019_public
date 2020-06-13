```bash

git config --global http.proxy 'socks5://127.0.0.1:xxxx'
git config --global https.proxy 'socks5://127.0.0.1:xxxx'

git config --global --unset http.proxy 'socks5://127.0.0.1:1086'
git config --global --unset https.proxy 'socks5://127.0.0.1:1086'


#只对github.com
git config --global http.https://github.com.proxy socks5://127.0.0.1:1086

#取消代理
git config --global --unset http.https://github.com.proxy
```
