# 2022-1-20

### p1

干什么的？
怎么用？

Web服务器

nginx是什么？能做什么事情？

反向代理
负载均衡
动静分离

服务器软件

80端口是默认宽口 可以省略不写

负载均衡

双击 会一闪而过 不建议 exe
80 默认端口 可以省略不写 

80 与8080区别

window nginx 基础命令
在Windows下使用Nginx，我们需要掌握一些基本的操作命令，比如：启动、停止Nginx服务，重新载入Nginx等，下面我就进行一些简单的介绍。(说明：打开cmd窗口) 
1、启动： 
C:\server\nginx-1.0.2>start nginx 
或 
C:\server\nginx-1.0.2>nginx.exe 
注：建议使用第一种，第二种会使你的cmd窗口一直处于执行中，不能进行其他命令操作。 
2、停止： 
C:\server\nginx-1.0.2>nginx.exe -s stop 
或 
C:\server\nginx-1.0.2>nginx.exe -s quit 
注：stop是快速停止nginx，可能并不保存相关信息；quit是完整有序的停止nginx，并保存相关信息。 
3、重新载入Nginx： 
C:\server\nginx-1.0.2>nginx.exe -s reload 
当配置信息修改，需要重新载入这些配置时使用此命令。 
4、重新打开日志文件： 
C:\server\nginx-1.0.2>nginx.exe -s reopen 
5、查看Nginx版本： 
C:\server\nginx-1.0.2>nginx -v 
nginx: nginx version: nginx/1.0.2 
或 
C:\server\nginx-1.0.2>nginx -V 

6、测试或载入指定配置文件： 
测试配置文件 
C:\server\nginx-1.0.2>nginx.exe -t -c conf/default.conf 
nginx: the configuration file C:\server\nginx-1.0.2/conf/default.conf syntax isok 
nginx: configuration file C:\server\nginx-1.0.2/conf/default.conf test is successful 
载入指定配置文件 
C:\server\nginx-1.0.2>start nginx.exe -c conf/default.conf

nginx -s reload

nginx.exe 一直出于执行中

nginx -s stop

 location / {

      root   html;  # 与nginx.exe 同级 指向根目录
      index  /html_test/index.html;

}

nginx 只成功了 生产环境的跨域解决 开发环境的跨域没有成功

https://www.cnblogs.com/lovesong/p/10269793.html
