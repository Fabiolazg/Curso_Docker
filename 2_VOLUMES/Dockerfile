FROM php:8-apache

WORKDIR /var/www/html/

COPY . .

# Garante que a pasta messages existe
RUN mkdir -p /var/www/html/messages

# Dá permissão total ao Apache
RUN chown -R www-data:www-data /var/www/html/messages
RUN chmod -R 775 /var/www/html/messages

EXPOSE 80