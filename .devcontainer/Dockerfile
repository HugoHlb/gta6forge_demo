FROM mcr.microsoft.com/devcontainers/php:8.4

RUN apt-get update \
    && apt-get install -y libicu-dev libzip-dev libpng-dev libjpeg-dev libfreetype6-dev libwebp-dev \
    && docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp \
    && docker-php-ext-install intl zip exif gd
