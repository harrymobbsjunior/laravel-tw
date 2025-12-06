FROM phpdockerio/php:8.4-fpm

# Diretório padrão da aplicação
WORKDIR /application

# Instala extensões essenciais para Laravel
RUN apt-get update && apt-get install -y --no-install-recommends \
        git \
        zip \
        unzip \
        curl \
        php8.4-mysql \
        php8.4-pgsql \
        php8.4-sqlite3 \
        php8.4-mbstring \
        php8.4-xml \
        php8.4-curl \
        php8.4-zip \
        php8.4-uuid \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*
