# Gunakan image khusus PHP 8.3 dari Microsoft (bukan Universal)
FROM mcr.microsoft.com/devcontainers/php:8.3

# Copy script installer sakti (mlocati)
COPY --from=mlocati/php-extension-installer /usr/bin/install-php-extensions /usr/local/bin/

# Install semua ekstensi Laravel yang Anda butuhkan
# Script ini otomatis mengurus dependency sistemnya
RUN install-php-extensions \
    gd \
    intl \
    pdo_mysql \
    zip \
    bcmath \
    redis \
    imagick \
    xml \
    curl \
    mbstring \
    opcache \
    sqlite3