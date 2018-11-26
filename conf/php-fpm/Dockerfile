FROM php:7.0-fpm-alpine
MAINTAINER oshou <adf1985adf@gmail.com>
USER root
RUN echo "install mysql mysqli pdo driver" \
    && docker-php-ext-install pdo pdo_mysql mysqli \
    && docker-php-ext-configure pdo_mysql --with-pdo-mysql=mysqlnd \
    && docker-php-ext-configure mysqli --with-mysqli=mysqlnd
