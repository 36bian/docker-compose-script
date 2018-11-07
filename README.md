### 注意
使用脚本前关闭selinux

### 使用方式
git clone 到本地，切进对应目录执行`docker-compose up -d`，执行前注意修改ip

### 各模块简介
* chfs：轻量级http文件共享服务器
* frpc：p2p穿透客户端，需配合服务端使用
* meow：局域网代理
* nginx：端口转发
* 云盘
  * pydio-cell，内存占用过高(1G)
