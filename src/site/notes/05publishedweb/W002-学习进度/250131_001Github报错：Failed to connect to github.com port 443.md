---
{"dg-publish":true,"permalink":"/05publishedweb/W002-学习进度/250131_001Github报错：Failed to connect to github.com port 443/","noteIcon":"","created":"2025-02-21T21:51:50.695+08:00","updated":"2025-02-21T22:04:22.474+08:00"}
---





[[03 科技or技能树/03-00_科技or技能树 索引\|03-00_科技or技能树 索引]]
解决方案：

[[01 日记/2025-01-31\|2025-01-31]]

遇到了一个443问题。说我连接github失败，目前已解决。原因是应用使用我的github时没有使用vpn代理，通过以下操作修改了github的端口号已解决：（我的vpn的端口号是10809）
```shell
git config --global http.proxy 127.0.0.1:10809 
git config --global https.proxy 127.0.0.1:10809
```
完毕后，可以使用下面命令来查询是否成功修改：
```shell
git config --global -l
```
参考资料：[Git报错： Failed to connect to github.com port 443 解决方案](https://blog.csdn.net/zpf1813763637/article/details/128340109)

