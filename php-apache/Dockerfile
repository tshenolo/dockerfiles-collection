# Use the official PHP image with Apache
FROM php:8.1-apache

# Set the working directory inside the container
WORKDIR /var/www/html

# Copy the current directory contents into the container
COPY . /var/www/html

# Install necessary PHP extensions
RUN docker-php-ext-install mysqli pdo pdo_mysql

# Set file permissions
RUN chown -R www-data:www-data /var/www/html

# Expose the Apache port
EXPOSE 80

# Start Apache in the foreground
CMD ["apache2-foreground"]