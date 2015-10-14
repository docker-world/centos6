FROM dockerworld/centos6:httpd

MAINTAINER Eric Mugerwa <ericmdev@gmail.com>

LABEL version="1.0"
LABEL description="PHP: 5.3 (MySQL; PDO; XML; Intl)"

# install php 5.3 - use default yum php - centos 6.7
RUN yum install php -y

# install php 5.3 extensions
RUN yum install php-pdo -y
RUN yum install php-mysql -y
RUN yum install php-mysqli -y
RUN yum install php-xml -y
RUN yum install php-intl -y
RUN yum install php-pecl-apc -y
RUN yum install php-fpm -y
RUN yum install php-cli -y

RUN rpm -Uvh http://dl.fedoraproject.org/pub/epel/5/i386/epel-release-5-4.noarch.rpm
RUN yum install php53-mcrypt -y

# RUN rpm -Uvh http://pkgs.org/centos-7/epel-x86_64/php-pecl-memcached-2.2.0-1.el7.x86_64.rpm.html
# RUN yum install php53-pecl-memcached -y

# yum clean all
RUN yum clean all
