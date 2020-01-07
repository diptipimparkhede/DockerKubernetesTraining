#Docker file for apache for Docker Kubernetes Training
FROM centos:7
MAINTAINER dips_pi@rediffmail.com
RUN yum -y update
ADD scripts /opt
RUN chmod 755 /opt/*
RUN /opt/packages
ADD code /var/www/html
#COPY code/* /var/www/html
ENV MY_DB_HOST_WRITE=test
EXPOSE 80
CMD ["httpd","-D","FOREGROUND"]