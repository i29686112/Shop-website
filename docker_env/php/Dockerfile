# Dockerfile
FROM php:8.1-fpm
WORKDIR /var
RUN apt-get update && apt-get install -y libpq-dev libpng-dev libzip-dev zip
RUN docker-php-ext-install pdo pdo_mysql gd zip\
&& docker-php-ext-enable opcache


# Install Composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
