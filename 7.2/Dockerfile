FROM alpine:3.7

# make sure you can use HTTPS
RUN apk add --update ca-certificates

# copy public key
ADD https://php.codecasts.rocks/php-alpine.rsa.pub /etc/apk/keys/php-alpine.rsa.pub

# add repositories
RUN echo "http://dl-cdn.alpinelinux.org/alpine/v3.7/main" > /etc/apk/repositories && \
    echo "http://dl-cdn.alpinelinux.org/alpine/v3.7/community" >> /etc/apk/repositories && \
    echo "@php http://php.codecasts.rocks/v3.7/php-7.2" >> /etc/apk/repositories

# remove cache and tmp files
RUN rm -rf /var/cache/apk/* && \
    rm -rf /tmp/*

# install Ansible, PHP, PHP extensions and necesary packages
RUN apk add --no-cache --update libressl \
    curl \
    ansible \
    php7@php \
    php7-openssl@php \
    php7-dev@php \
    php7-common@php \
    php7-apcu@php \
    php7-bcmath@php \
    php7-ctype@php \
    php7-curl@php \
    php7-exif@php \
    php7-iconv@php \
    php7-intl@php \
    php7-json@php \
    php7-mbstring@php \
    php7-opcache@php \
    php7-pcntl@php \
    php7-pdo@php \
    php7-mysqlnd@php \
    php7-pdo_mysql@php \
    php7-pdo_pgsql@php \
    php7-phar@php \
    php7-posix@php \
    php7-session@php \
    php7-xml@php \
    php7-xsl@php \
    php7-zip@php \
    php7-zlib@php \
    php7-dom@php \
    php7-redis@php \
    php7-fpm@php \
    php7-xdebug@php

# create symlink for php7
RUN ln -sf /usr/bin/php7 /usr/bin/php

# install Composer.
RUN curl -sS https://getcomposer.org/installer | php \
  && chmod +x composer.phar && mv composer.phar /usr/local/bin/composer
