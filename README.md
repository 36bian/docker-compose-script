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
  * kod-explorer：php开发，小巧易用，但处理大文件不佳
  * pydio-cell：go开发，简洁、功能强，但内存占用过高(1G)

