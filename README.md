<h1> Contruindo um projeto de arquitetura baseada em microsserviços usando Spring Cloud </h1>

Uma _live coding_ em que foi desenvolvido um pequeno sistema de e-commerce usando uma arquitetura de microsserviços, através do elasticsearch.

Durante as aulas foram desenvolvidos e abordados os seguintes tópicos:

* Setup inicial de projeto com o Spring Boot Initialzr
* Criação de modelo de dados para mapeamento de entidades em banco de dados do product-catalog
* Criação de modelo de dados para mepeamento de entidades em banco de dados do shopping-cart
* Implementação do elasticSearch via docker
* Implementação do banco de dados Redis via Docker
* Criação de config-server para conectar as aplicações
* Adição da dependência config-client para a conexão das aplicações
* Implementação do catálogo de serviços (service-discovery) Eureka
* Implementação do gateway


Para executar o backend no terminal, digite o comando:

```shell script
gradlew run
```

Catálogo de serviços ficarão na porta 9000
```uri
http://localhost:9000
```

Acesso ao backend pelo navegador:

```uri
http://localhost:8888
```
 

Com isso, o projeto pode ser acessado pelo endereço:

```uri
http://localhost:4200/
```

O que eu utilizei para acompanhar este projeto:

* CRUD REST API:
  * Spring Boot 2.2.6
  * Java 8
  * Gradle 7.2
* Outros Apps de suporte:
  * VSCode 1.60.0
  * NodeJs 12.22.5
  * Npm 6.14.14
  * Controle de versão GIT
  * Conta GITHUB para armazenamento do projeto