# Especifica a imagem de origem
FROM ubuntu

# Instala os pacotes
RUN apt-get update
RUN DEBIAN_FRONTEND="noninteractive" apt-get -y install tzdata 
RUN apt-get install -y \
    apache2 \
 && rm -rf /var/lib/apt/lists/*

# Copia o arquivo html
COPY ./index.html /var/www/html/
 
# Expõe a porta do apache
EXPOSE 80
 
# Executa o apache
CMD ["/usr/sbin/apache2ctl", "-DFOREGROUND"]
