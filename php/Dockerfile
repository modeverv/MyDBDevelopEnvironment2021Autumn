FROM php:8.0-fpm

RUN apt-get update \
    && docker-php-ext-install pdo_mysql 
RUN apt-get install -y libpq-dev \
    && docker-php-ext-configure pgsql -with-pgsql=/usr/local/pgsql \
    && docker-php-ext-install pdo pdo_pgsql pgsql
    