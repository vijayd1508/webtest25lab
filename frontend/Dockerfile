FROM centos:latest
MAINTAINER vijayd1508@gmail.com
RUN yum -y update
ADD config /opt/
RUN yum -y install `cat /opt/packages`
ADD code /var/www/html/
EXPOSE 80
CMD ["apachectl","-D","FOREGROUND"]