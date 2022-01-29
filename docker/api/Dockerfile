FROM php:8.0-fpm

ENV TZ Asia/Tokyo

# install Library
RUN apt-get update && \
	apt-get install -y git && \
	docker-php-ext-install pdo_mysql 
		
# config file COPY
COPY ./docker/api/php.ini /usr/local/etc/php/php.ini

# install Composer
COPY --from=composer:2.0 /usr/bin/composer /usr/bin/composer

WORKDIR /app