FROM mcr.microsoft.com/devcontainers/universal:2

# Install PHP Extensions manually
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends \
    php8.3-gd \
    php8.3-intl \
    php8.3-mysql \
    php8.3-zip \
    php8.3-bcmath \
    php8.3-redis \
    php8.3-imagick \
    php8.3-xml \
    php8.3-curl \
    php8.3-mbstring \
    && apt-get clean -y && rm -rf /var/lib/apt/lists/*