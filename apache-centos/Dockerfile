
FROM centos:7

LABEL maintainer="vipin2411@gmail.com"

RUN yum -y update && yum -y install httpd && yum clean all

ADD index.html /var/www/html/index.html

EXPOSE 80

ENTRYPOINT ["/usr/sbin/httpd","-D","FOREGROUND"]

