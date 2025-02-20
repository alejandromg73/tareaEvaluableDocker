# Uso la imagen base oficial de PHP con Apache
FROM php:7.4-apache

# Copio los archivos del sitio web al directorio raíz de Apache
COPY index.html /var/www/html/
COPY estilos.css /var/www/html/
COPY script.php /var/www/html/

# Expongo el puerto 8000 para el servidor web
EXPOSE 8000

# Inicio Apache en segundo plano y redireccionar al puerto 8000
CMD ["apachectl", "-D", "FOREGROUND"]