FROM php:5.6-apache
MAINTAINER M Parker <mparker17@536298.no-reply.drupal.org>

ENV REFRESHED_AT 2015-01-02

RUN apt-get update && apt-get install -y libpng12-dev php5-common && rm -rf /var/lib/apt/lists/* \
    && docker-php-ext-install gd \
    && apt-get purge --auto-remove -y libpng12-dev
RUN docker-php-ext-install mysqli pdo_mysql
RUN docker-php-ext-install mbstring
