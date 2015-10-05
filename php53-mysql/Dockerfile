FROM dockerworld/centos6:php53

MAINTAINER Eric Mugerwa <ericmdev@gmail.com>

LABEL version="1.0"
LABEL description="PHP 5.3 w. MySQL"

# install mysql
RUN yum install mysql-server -y
RUN chkconfig --level 345 mysqld on

EXPOSE 3306