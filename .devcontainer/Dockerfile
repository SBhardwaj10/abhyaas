FROM mcr.microsoft.com/devcontainers/php:8.2

RUN apt-get update && apt-get install -y nodejs npm git unzip \
    && npm install -g npm@latest \
    && npm install -g yarn \
    && curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer \
    && composer global require laravel/installer

WORKDIR /workspaces/ulearn-lms
