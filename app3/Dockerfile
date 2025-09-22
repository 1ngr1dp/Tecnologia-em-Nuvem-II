# Use a imagem oficial do PHP com Apache
FROM php:7.4-apache

# Ativa mod_rewrite no Apache
RUN a2enmod rewrite

# Copia o código PHP para o diretório público do Apache
COPY ./index.php /var/www/html/

# Define as permissões corretas para os arquivos
RUN chown -R www-data:www-data /var/www/html

# Expõe a porta 80
EXPOSE 80

# Inicia o Apache no foreground
CMD ["apache2-foreground"]

