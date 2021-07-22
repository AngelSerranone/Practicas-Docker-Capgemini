##Para pasarle por argumento el sistema que quiero que me instale

##Descargamos UBUNTU
FROM ubuntu

## Argumentos a pasarle
ARG installer=python

## hay que hacer update antes de nada
RUN apt-get update

## Se le pasa el argumento
RUN apt-get install -y ${installer}