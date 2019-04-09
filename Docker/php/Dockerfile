FROM php:7.3-fpm

RUN apt-get -y update && apt-get -y install libfreetype6-dev libjpeg62-turbo-dev libpng-dev libzip-dev mariadb-client
RUN docker-php-ext-configure zip --with-libzip=/usr/include \
	&& docker-php-ext-configure gd --with-freetype-dir=/usr/include --with-jpeg-dir=/usr/include
RUN docker-php-ext-install pdo_mysql zip mbstring gd

COPY php.ini $PHP_INI_DIR/conf.d/
