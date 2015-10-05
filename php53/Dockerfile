FROM dockerworld/centos6:httpd

MAINTAINER Cein Markey <hi@ceinmarkey.co.uk>

LABEL version="1.0"
LABEL description="PHP: 5.3 (PDO, MySQLI, XML, Intl)"

# install php 5.3
RUN rpm -Uvh https://dl.fedoraproject.org/pub/epel/epel-release-latest-6.noarch.rpm
RUN rpm -Uvh https://mirror.webtatic.com/yum/el6/webtatic-release.rpm
RUN yum install php53w php53w-opcache -y

# install php 5.3 extensions
RUN yum install php53w-pdo -y
RUN yum install php53w-mysqli -y
RUN yum install php53w-xml -y
RUN yum install php53w-intl -y

# set php date timezone
RUN perl -pi -e "s#;date.timezone =.*#date.timezone = Europe/London#g" /etc/php.ini

# yum clean all
RUN yum clean all