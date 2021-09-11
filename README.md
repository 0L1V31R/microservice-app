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
Sequência de inicialização:
1. Config-server
2. Service-discovery
3. Gateway
4. Product-catalog e Shopping-cart não tem preferência


O catálogo de serviços ficará na porta 9000
```uri
http://localhost:9000
```
O Gateway fará o balanceamento dos serviços registrads no catálogo para que a aplicação REST possa funcionar.

O que eu utilizei para acompanhar este projeto foi:

* CRUD REST API:
  * Spring Boot 2.2.6
  * Java 8
  * Gradle 7.2
  * Redis
  * ElasticSearch
* Outros Apps de suporte:
  * VSCode 1.60.0
  * Controle de versão GIT
  * Conta GITHUB para armazenamento do projeto