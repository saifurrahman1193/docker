# container built up with that image
FROM php:7.4-fpm-alpine

RUN docker-php-ext-install pdo pdo_mysql

# # Set working directory
# WORKDIR /var/www

# # Copy composer.lock and composer.json
# COPY composer.lock composer.json /var/www/


# # Install dependencies
# RUN apt-get update && apt-get install -y \
#     build-essential libpng-dev libjpeg62-turbo-dev libfreetype6-dev locales \
#     zip jpegoptim optipng pngquant gifsicle vim unzip git curl build-essential \
#     software-properties-common wget  libwebp-dev

# # Add docker php ext repo
# ADD https://github.com/mlocati/docker-php-extension-installer/releases/latest/download/install-php-extensions /usr/local/bin/

# RUN chmod +x /usr/local/bin/install-php-extensions && sync && \
#     install-php-extensions mbstring pdo_mysql exif pcntl gd memcached

# # RUN docker-php-ext-install zip mysqli mbstring pdo pdo_mysql tokenizer xml bcmath opcache pcntl intl soap exif gd

# # Clear cache
# RUN apt-get clean && rm -rf /var/lib/apt/lists/*

# # Install extensions
# # RUN docker-php-ext-install pdo_mysql mbstring zip exif pcntl
# # RUN docker-php-ext-configure gd --with-gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ --with-png-dir=/usr/include/
# RUN docker-php-ext-install gd

# # Install composer
# RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# # Add user for laravel application
# RUN groupadd -g 1000 www
# RUN useradd -u 1000 -ms /bin/bash -g www www

# # Copy existing application directory contents
# COPY . /var/www

# # Copy existing application directory permissions
# COPY --chown=www:www . /var/www

# # Change current user to www
# USER www

# # Expose port 9000 and start php-fpm server
# EXPOSE 80
# CMD ["php-fpm"]
