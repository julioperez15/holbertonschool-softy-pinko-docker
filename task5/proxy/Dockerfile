# Usar la última imagen de Nginx como base
FROM nginx:latest

# Copiar el archivo de configuración de Nginx para el proxy
COPY ./proxy.conf /etc/nginx/conf.d/default.conf

# Exponer el puerto 80 que usará Nginx
EXPOSE 80
