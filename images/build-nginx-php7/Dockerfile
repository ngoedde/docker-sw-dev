FROM jeboehm/php-nginx-base

COPY config/nginx.conf /etc/nginx

WORKDIR /var/www/html

RUN echo http://dl-2.alpinelinux.org/alpine/edge/community/ >> /etc/apk/repositories \
    && apk --no-cache add shadow && usermod -u 1000 www-data \
    && chown -R www-data /var/www