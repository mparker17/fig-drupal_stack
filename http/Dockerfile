FROM php:5.6-apache
MAINTAINER M Parker <mparker17@536298.no-reply.drupal.org>

ENV REFRESHED_AT 2015-01-02

RUN apt-get update && apt-get install -y re2c libpng12-0 libpng12-dev libpng3 \
        && docker-php-ext-install gd && docker-php-ext-install mbstring
