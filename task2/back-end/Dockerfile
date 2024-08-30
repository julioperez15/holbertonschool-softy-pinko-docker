# Usar la última imagen de Ubuntu como base
FROM ubuntu:latest

# Actualizar los repositorios de APT y el software instalado
RUN apt-get update && apt-get upgrade -y

# Instalar Python3 y pip3
RUN apt-get install -y python3 python3-pip

# (Opcional) Eliminar archivo EXTERNALLY-MANAGED si es necesario
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED || true

# Instalar Flask usando pip3
RUN pip3 install flask

# Establecer el directorio de trabajo a /app
WORKDIR /app

# Copiar el archivo api.py al directorio de trabajo
COPY ./api.py /app/api.py

# Exponer el puerto 5252 del contenedor
EXPOSE 5252

# Comando por defecto para ejecutar la aplicación Flask
CMD ["python3", "/app/api.py"]
