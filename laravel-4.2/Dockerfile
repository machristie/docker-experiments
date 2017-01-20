FROM centos:7

RUN yum -y update && yum -y install epel-release && yum -y install \
        composer \
        httpd \
        php \
        php-mcrypt \
        php-soap \
    && yum clean all

EXPOSE 80

VOLUME /var/www/html

CMD ["/usr/sbin/httpd", "-DFOREGROUND"]
