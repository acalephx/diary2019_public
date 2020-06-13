```bash

git config --global http.proxy 'socks5://127.0.0.1:1086'
git config --global https.proxy 'socks5://127.0.0.1:1086'

git config --global --unset http.proxy 'socks5://127.0.0.1:1086'
git config --global --unset https.proxy 'socks5://127.0.0.1:1086'


#只对github.com
git config --global http.https://github.com.proxy socks5://127.0.0.1:1080

#取消代理
git config --global --unset http.https://github.com.proxy
————————————————
版权声明：本文为CSDN博主「isea533」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/isea533/article/details/84748009

```
