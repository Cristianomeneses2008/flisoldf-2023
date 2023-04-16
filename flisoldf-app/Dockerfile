### STAGE 1:BUILD ###
# Instalando um node
FROM node:12.14-alpine AS build
# Create a Virtual directory inside the docker image
WORKDIR /user/app
# Copy files to virtual directory
COPY package.json package-lock.json ./
# Run command in Virtual directory
RUN npm install
# Copy files from local machine to virtual directory in docker image
COPY . .
# porta
EXPOSE 3333
#executar os comandos dentro do container
CMD ['npm', 'run', 'dev']