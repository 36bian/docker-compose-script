### 配置文件写法

服务器配置文件写法 frps.ini：
```shell
[common]
bind_port = 7000
vhost_http_port = 80
```

客户端配置文件写法 frpc.ini
```shell
[common]
server_addr = 服务器ip
server_port = 7000

[web]
type = http
local_ip = 宿主ip # 因为处在docker容器中所以这里要改一下
local_port = 80 # nginx端口
custom_domains = *.example.com
```

### 简介
万网配置泛域名解析到vps，frps直接监听服务器80端口，不用起nginx。
客户端配置frpc泛域名解析到本地nginx80端口，剩下的都交给nginx处理

### 缺点
不支持https
