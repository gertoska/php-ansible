FROM alpine:3.5

# install Ansible, PHP, PHP extensions and necesary packages
RUN apk add --no-cache --update ansible \
    bash \
    curl \
    git \
    libressl \
    nodejs \
    openssh \
    php5 \
    php5-apcu \
    php5-bcmath \
    php5-common \
    php5-ctype \
    php5-curl \
    php5-dev \
    php5-dom \
    php5-exif \
    php5-fpm \
    php5-gd \
    php5-iconv \
    php5-intl \
    php5-json \
    php5-opcache \
    php5-openssl \
    php5-pcntl \
    php5-pdo \
    php5-pdo_mysql \
    php5-pdo_pgsql \
    php5-phar \
    php5-posix \
    php5-sockets \
    php5-xdebug \
    php5-xml \
    php5-xsl \
    php5-zip \
    php5-zlib

# install Composer.
RUN curl -sS https://getcomposer.org/installer | php \
  && chmod +x composer.phar && mv composer.phar /usr/local/bin/composer
