# Use an official PHP runtime as a parent image
FROM php:apache

# Install PHP extensions and other dependencies
RUN apt-get update && \
    apt-get install -y libpng-dev && \
    docker-php-ext-install pdo pdo_mysql gd mysqli && \
    rm -rf /var/lib/apt/lists/*

# Copy your PHP application code into the container
COPY mysql.php /var/www/html/

# Expose the port Apache listens on
EXPOSE 80

# Start Apache when the container runs
CMD ["apache2-foreground"]
