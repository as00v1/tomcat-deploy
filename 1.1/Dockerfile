FROM tomcat:8
LABEL version="1.1" maintainer="jiayong <superjiayong@qq.com>"
ADD server.xml /usr/local/tomcat/conf/
ADD tomcat-users.xml /usr/local/tomcat/conf/
ADD manager.xml /usr/local/tomcat/conf/Catalina/localhost/
ADD catalina.sh /usr/local/tomcat/bin/
#设置时区
RUN /bin/cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
  && echo 'Asia/Shanghai' >/etc/timezone \
CMD ["catalina.sh", "run"]