FROM 4xxi/php:flex

RUN apt-get update && apt-get install -y \
    libpq-dev

RUN docker-php-ext-install \
    pdo_pgsql

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer && \
    chmod +x /usr/local/bin/composer && \
    composer global require hirak/prestissimo  --no-interaction