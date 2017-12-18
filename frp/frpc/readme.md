# 启动

>docker run --rm -h="frpc-docker" --name frpc-docker -v $(pwd)/frpc.ini:/usr/local/frpc/frpc.ini budblack/frpc-docker:latest


# frpc.default.ini

```ini
[common]
server_addr = frps.atech.ltd
server_port = 9561
privilege_token = budblack

#pool_count = 5
#tcp_mux = true
#user = admin
#login_fail_exit = false
#protocol = tcp

#[tmp.1.http]
#type = http
#local_ip = 192.168.19.153
#local_port = 80
#use_encryption = true
#use_compression = true
#custom_domains = http.1.tmp.domain.com

[tmp.0.ssh]
type        = tcp
local_ip    = 127.0.0.1
local_port  = 22
remote_port = 9571
```


# 已知问题

## authorization timeout
可能是客户端时间与服务器时间差异过大, 这个问题普遍出现在mac端的docker里. 重启笔记本就好