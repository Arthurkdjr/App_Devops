# Utilise une image PHP avec Apache
FROM php:7.4-apache
WORKDIR /var/www/html

# Copie les fichiers PHP
COPY package.json package-lock.json ./

# Installe les extensions PHP nécessaires
RUN docker-php-ext-install pdo_mysql

# Expose le port 80
EXPOSE 80

# Démarre Apache
CMD ["apache2-foreground"]