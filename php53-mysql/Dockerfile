FROM dockerworld/centos6:php53

MAINTAINER Cein Markey <hi@ceinmarkey.co.uk>

LABEL version="1.0"
LABEL description="MySQL"

# install mysql
RUN yum install mysql -y
RUN yum install mysql-server -y
RUN chkconfig --level 345 mysqld on

EXPOSE 3306