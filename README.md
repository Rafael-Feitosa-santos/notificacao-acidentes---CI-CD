# Notificação de Acidentes - CI/CD

Este repositório contém uma aplicação para notificação de acidentes, utilizando Java, Spring Boot, Maven, Docker e integração contínua (CI/CD).

## Requisitos

Antes de começar, certifique-se de ter os seguintes requisitos instalados:

- [Docker](https://www.docker.com/get-started)
- [Java 22](https://jdk.java.net/22/)
- [Maven 3.9.9](https://maven.apache.org/download.cgi)
- [Git](https://git-scm.com/)

## Como rodar a aplicação

### 1. Clonar o repositório

Clone o projeto para sua máquina local usando Git:

```sh
git clone https://github.com/usuario/notificacao-acidentes.git
cd notificacao-acidentes--CI-CD
```

### Compilar o projeto com Maven

No diretório do projeto, execute o seguinte comando para compilar o código e construir o pacote JAR:

``` sh
mvn clean install
```

### Construir a imagem Docker
Agora que o projeto está compilado, você pode construir a imagem Docker:

``` sh
docker build -t notificacao-acidentes .
```

### Rodar a aplicação com Docker
Para executar a aplicação dentro de um container Docker, utilize o comando:

``` sh
docker run -d --name notificacao-acidentes -p 8080:8080 notificacao-acidentes
```

###  Rodar com Docker Compose

``` sh
docker-compose up
```