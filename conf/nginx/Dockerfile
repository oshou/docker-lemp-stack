FROM nginx:1.13.5-alpine
RUN echo "set timezone" \
    && apk add --update tzdata \
    && cp /usr/share/zoneinfo/Asia/Tokyo /etc/localtime \
    && apk del tzdata \
    && rm -rf /var/cache/apk
