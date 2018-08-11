FROM php:7-fpm-alpine
USER root
RUN echo "set timezone" \
    && apk add --update tzdata \
    && cp /usr/share/zoneinfo/Asia/Tokyo /etc/localtime \
    && apk del tzdata \
    && echo "install mysql mysqli pdo driver" \
    && docker-php-ext-install mysqli pdo pdo_mysql \
    && rm -rf /var/cache/apk
