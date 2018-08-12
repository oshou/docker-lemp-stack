FROM nginx:1.15.2-alpine
USER root
RUN echo "set timezone" \
    && apk add --update --no-cache tzdata \
    && cp /usr/share/zoneinfo/Asia/Tokyo /etc/localtime \
    && apk del tzdata
