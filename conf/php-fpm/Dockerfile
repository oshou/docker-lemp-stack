FROM php:7-fpm-alpine
USER root
RUN echo "set timezone" \
    && apk add --update --no-cache tzdata \
    && cp /usr/share/zoneinfo/Asia/Tokyo /etc/localtime \
    && apk del tzdata
RUN echo "install mysql mysqli pdo driver" \
    && docker-php-ext-install pdo_mysql mysqli mbstring
