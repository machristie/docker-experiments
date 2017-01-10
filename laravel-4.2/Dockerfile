FROM centos:7

RUN yum -y update && yum -y install epel-release && yum -y install \
        composer \
        httpd \
        php \
        php-mcrypt \
        php-soap \
    && yum clean all

COPY ./simple-laravel /var/www/html
RUN chown -R apache:apache /var/www/html/app/storage

EXPOSE 80

VOLUME /var/www/html

CMD ["/usr/sbin/httpd", "-DFOREGROUND"]
