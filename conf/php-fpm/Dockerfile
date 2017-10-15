FROM php:7-fpm-alpine
RUN echo "set timezone" \
    && apk add --update tzdata \
    && cp /usr/share/zoneinfo/Asia/Tokyo /etc/localtime \
    && apk del tzdata \
    && rm -rf /var/cache/apk \
    echo "install mysql mysqli pdo driver" \
    && docker-php-ext-install mysqli pdo pdo_mysql
