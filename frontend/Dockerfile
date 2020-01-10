#Docker file for apache for Docker Kubernetes Training
FROM centos:7
MAINTAINER dips_pi@rediffmail.com
RUN yum -y update
RUN yum -y install http php php-gd php-mysql
ADD code /var/www/html
#COPY code/* /var/www/html
ENV MY_DB_HOST_WRITE=mysql-0.mysql
EXPOSE 80
CMD ["httpd","-D","FOREGROUND"]