FROM nginx:1.13.2
MAINTAINER budblack@qq.com

EXPOSE 80 9599 9598 9597

ADD ./nginx.conf /etc/nginx/nginx.conf
ADD ./htpasswd /etc/nginx/htpasswd

ADD ./io.tool.budblack.me.crt /etc/nginx/io.tool.budblack.me.crt
ADD ./io.tool.budblack.me.key /etc/nginx/io.tool.budblack.me.key

ADD ./ydtx.bianbiankj.com.crt /etc/nginx/ydtx.bianbiankj.com.crt
ADD ./ydtx.bianbiankj.com.key /etc/nginx/ydtx.bianbiankj.com.key
