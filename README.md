# dockerfile_gitpod
Dockerfile Ubuntu, PHP, SQLite3

# Comandos

## Ejecutar dockerfile
docker build -t php:v1 .

## Visualizar imagenes creadas
docker images

## Crear contenedor
docker run -it -p 8080:8080 -v /workspace/dockerfile_gitpod/images:/images --name webapp -h webapp php:v1

## Visualizar nuestro contenedor
docker ps -a

## Ejecutar php desde terminal
php -S 0.0.0.0:8080 -t .