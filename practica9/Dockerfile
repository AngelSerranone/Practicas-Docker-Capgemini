##Para instalar Solr

## descargo centos
FROM centos
## instalar java
RUN yum -y update
RUN yum -y install java-1.8.0-openjdk.x86_64
RUN yum -y install wget
## instalar lsof porque lo necesita
RUN yum -y install lsof

## instalar Solr
WORKDIR /opt
RUN wget https://downloads.apache.org/lucene/solr/8.9.0/solr-8.9.0.tgz
RUN tar xzf solr-8.9.0.tgz

## Exponemos un puerto de entrada
EXPOSE 8983

## Ejecutamos un comando final
ENTRYPOINT ["/opt/solr-8.9.0/bin/solr", "start", "-force", "-f"]


## PARA MONTAR LA IMAGEN: docker build -t angelserranone/solr .
## PARA HACER EL RUN: docker run -d --name solr1 -p 8983:8983 angelserranone/solr