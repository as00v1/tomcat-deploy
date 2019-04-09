# 一、tomcat-deploy是什么？
tomcat-deploy是基于官方版tomcat8制作的支持自动部署的docker镜像源码。默认部署用户的用户名密码均为deploy。

# 二、docker hub地址
访问这个地址在docker hub中查看：  
<https://cloud.docker.com/u/as00v1/repository/docker/as00v1/tomcat-deploy>

# 三、使用方法
## 1.直接下载镜像
在docker环境下，执行：
```
docker pull as00v1/tomcat-deploy:1.1
```
## 2.本地编译
将项目clone至本地，在包含Dockerfile文件的目录执行：
```
docker build -t yourname/tomcat-deploy:1.1
```
---
# 更新日志
## 2019年4月9日

### 1.1：

* 解决了容器日期、tomcat日期不是东八区的问题  

建议直接pull 1.1版本就好

## 2019年4月8日
### 1.0：

* 初始版本，设置tomcat远程GUI用户的用户名密码均为gui，部署用户的用户名密码为deploy