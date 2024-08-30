# Usar la última imagen de Nginx como base
FROM nginx:latest

# Copiar los archivos del front-end al directorio adecuado en la imagen de Nginx
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copiar el archivo de configuración de Nginx
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Exponer el puerto 9000 para acceso
EXPOSE 9000
