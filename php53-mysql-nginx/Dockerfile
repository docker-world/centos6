FROM dockerworld/centos6:base

MAINTAINER Cein Markey <hi@ceinmarkey.co.uk>

LABEL version="1.0"
LABEL description="php53-mysql-nginx"

RUN yum install epel-release -y
RUN yum install nginx -y

RUN yum install php-5.3.3-46.el6_6.x86_64 -y
RUN yum install php-pdo -y
RUN yum install php-mysqli -y
RUN yum install php-xml -y
RUN yum install php-intl -y

RUN yum install mysql-server-5.1.73-5.el6_6.x86_64 -y

RUN yum clean all