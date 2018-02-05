## HTML5-Based Speedtest on Docker

### 0. 特别说明

* 由于Speedtest会尽可能使用最大的带宽，来反馈最真实的网络性能，所以，在部署完成项目后，**请不要将你的测速地址分享给其他人或者公开到群/论坛/贴吧等处！** 因此导致的流量损失、超流量停机，甚至欠费，iLemonrain (以下简称镜像作者)将不负任何责任！

### 1. 镜像说明
[网页版Speedtest](http://www.speedtest.net/) 却测试不出来本地到目标服务器的速度？  
  
服务器上跑 Speedtest-CLI 却总感觉测试结果不靠谱？  
  
现在，有了 [HTML5-Based Speedtest on Docker](https://hub.docker.com/r/ilemonrain/html5-speedtest/) ，这一切都迎刃而解！  
  
(更要命的是居然还Docker化了？真正的一键部署测速环境！)  
  
### 2. 镜像Tag
**Docker镜像**：ilemonrain/html5-speedtest  
```html5-speedtest```, ```html5-speedtest:latest```：默认Speedtest镜像，默认为Alpine Linux内核  
```html5-speedtest:alpine```：Alpine Linux内核

### 3. 使用方法
**启动命令行**：  
```docker run [-t/-d] -p [6688]:80 ilemonrain/html5-speedtest:latest```  

> **-t**：启动后显示日志，可用Ctrl+C转入后台运行  
> **-d**：后台模式启动  
> **-p 6688:80**：镜像映射端口，修改6688为任意端口即可
  
之后访问 ```http://你的服务器IP地址:镜像映射端口/``` ，即可愉快的开始测速啦~

### 4. 更新日志
#### Release 2018/02/05
> 镜像发布  

### 5. 联系作者
Email到ilemonrain@ilemonrain.com