FROM php:8.1-apache

COPY . /var/www/html/

RUN chown -R www-data:www-data /var/www/html/ \
    && chmod -R u=rwX,g=rX,o= /var/www/html/

WORKDIR /var/www/html

RUN apt-get update -y && apt-get install -y libmariadb-dev 
RUN docker-php-ext-install mysqli



