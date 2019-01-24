## PHP Ansible Dockerfile
[![Docker Pulls](https://img.shields.io/docker/pulls/gertoska/php-ansible.svg)](https://hub.docker.com/r/gertoska/php-ansible/)

This dockerfile extends from [Alpine image](https://hub.docker.com/_/alpine/). Intended for use in a CI environment.

#### Images:

|    Tag     | Parent     |Image Layers
|------------|------------|---------
| [7.2](https://github.com/gertoska/php-ansible/blob/master/7.2/Dockerfile)        |   alpine:3.7   | [![](https://images.microbadger.com/badges/image/gertoska/php-ansible:7.2.svg)](https://microbadger.com/images/gertoska/php-ansible:7.2 "Get your own image badge on microbadger.com")
| [5.6](https://github.com/gertoska/php-ansible/blob/master/5.6/Dockerfile)        |   alpine:3.5   | [![](https://images.microbadger.com/badges/image/gertoska/php-ansible:5.6.svg)](https://microbadger.com/images/gertoska/php-ansible:5.6 "Get your own image badge on microbadger.com")

#### Docker images contains:

* PHP (7.2 or 5.6)
* Ansible (latest)
* Composer (lastest)

####  PHP extensions:

* apcu
* bcmath
* common
* ctype
* curl
* dev
* dom
* exif
* fpm
* gd
* iconv
* intl
* json
* mbstring
* mysqlnd
* opcache
* openssl
* pcntl
* pdo
* pdo_mysql
* pdo_pgsql
* phar
* posix
* redis
* session
* sockets
* xdebug
* xml
* xsl
* zip
* zlib

#### Other packages

* bash
* curl
* nodejs
* npm
* openssh
