## Dockerfile

Exemplo de como criar um container usando Dockerfile para hospedar um servidor Web estático.

Entrar no diretório onde se encontra o arquivo Dockerfile e criar uma imagem:

<pre>
docker build -t webserver .
</pre>

Listar as imagens:

<pre>
docker images
</pre>

Executar o container:

<pre>
docker run -t -d -p 80:80 webserver
</pre>

Para testar, se estiver executando o container localmente, acesar diretamente o endereço localhost:

* http://localhost


Para mais informações, acessar a página da Wiki [Trabalhando com containers no Docker](https://github.com/mvneves/docker-examples/wiki/Trabalhando-com-containers-no-Docker)
