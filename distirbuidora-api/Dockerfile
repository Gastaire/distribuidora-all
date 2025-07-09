# Usamos una imagen oficial de Node.js como base.
# 'alpine' es una versión ligera, ideal para producción.
FROM node:18-alpine

# Establecemos el directorio de trabajo dentro del contenedor.
WORKDIR /usr/src/app

# Copiamos los archivos de dependencias. El '*' asegura que tanto
# package.json como package-lock.json se copien.
COPY package*.json ./

# Instalamos las dependencias del proyecto.
RUN npm install

# Copiamos el resto de los archivos de nuestra aplicación al directorio de trabajo.
COPY . .

# Exponemos el puerto en el que correrá nuestra API.
# Debe coincidir con el puerto que definimos en el archivo .env
EXPOSE 4000

# El comando que se ejecutará cuando el contenedor se inicie.
CMD [ "node", "index.js" ]
