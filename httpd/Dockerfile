FROM dockerworld/centos6:base

MAINTAINER Cein Markey <hi@ceinmarkey.co.uk>

LABEL version="1.0"
LABEL description="Httpd"

RUN yum install httpd -y
RUN chkconfig httpd on
RUN perl -pi -e "s/EnableSendfile on/EnableSendfile off/g" /etc/httpd/conf/httpd.conf
RUN yum clean all

EXPOSE 80
EXPOSE 443