# Usamos una imagen oficial y ligera de Nginx, que es un servidor web muy eficiente.
FROM nginx:1.21.6-alpine

# Copiamos nuestro archivo index.html a la carpeta que Nginx sirve por defecto.
COPY index.html /usr/share/nginx/html/index.html

# Exponemos el puerto 80, que es el puerto estándar para HTTP.
EXPOSE 80

# El comando por defecto de la imagen de Nginx ya es iniciar el servidor,
# por lo que no necesitamos un CMD explícito.
