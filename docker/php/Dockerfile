FROM php:7.2.8-fpm
COPY php.ini /usr/local/etc/php/

RUN cd /usr/bin && curl -s http://getcomposer.org/installer | php && ln -s /usr/bin/composer.phar /usr/bin/composer

RUN apt-get update \
    && apt-get install -y \
    git \
    zip \
    unzip \
    vim

WORKDIR /var/www
