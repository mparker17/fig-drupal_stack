FROM php:5.6-apache
MAINTAINER M Parker <mparker17@536298.no-reply.drupal.org>

ENV REFRESHED_AT 2015-01-02

RUN apt-get -y update && apt-get install -y libpng12-dev php5-gd
RUN docker-php-ext-install gd mbstring
