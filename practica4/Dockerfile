FROM ubuntu:18.04 
ENV LENGUAJE python
RUN apt-get update
RUN apt-get install -y "$LENGUAJE"
RUN apt-get install -y wget
RUN mkdir /tmp/ejemplo 
COPY prueba.txt /tmp/ejemplo
CMD [ "cat", "/temp/ejemplo/ejemplo.txt" ]