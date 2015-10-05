FROM dockerworld/centos6:httpd

MAINTAINER Eric Mugerwa <ericmdev@gmail.com>

LABEL version="1.0"
LABEL description="PHP: 5.3 (MySQL; PDO; XML; Intl)"

# install php 5.3 - use default yum php - centos 6.7
RUN yum install php -y

# install php 5.3 extensions
RUN yum install php-pdo -y
RUN yum install php-mysqli -y
RUN yum install php-xml -y
RUN yum install php-intl -y

# set php date timezone
RUN perl -pi -e "ys#;date.timezone =.*#date.timezone = Europe/London#g" /etc/php.ini

# yum clean all
RUN yum clean all