# Lojinha API Automação

Este é um repositório que contém a automação de alguns testes de API Rest de um software denominado de Lojinha. Os sub-tópicos abaixo descrevem algumas decisões tomadas na estruturação do projeto.


## Tecnologias Utilizadas

- Java
  https://www.oracle.com/br/java/technologies/downloads/#jdk20-windows

- JUnit
  https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-api/5.8.0-M1

- RestAssured
  https://mvnrepository.com/artifact/io.rest-assured/rest-assured/4.4.0

- Maven
  https://maven.apache.org/

## Testes Automatizados
Testes para validar as partições de equivalência relacionadas ao valor do produto na lojinha, que estão vinculados diretamente a regra de negócio que diz que o valor do produto deve estar entre R$ 0,01 e R$ 7.000,00.

## Notas Gerais

- Sempre utilizamos anotação Before Each para capturar o token que será utilizado posteriormente nos métodos de testes.
- Armazenamos os dados que são enviados para API através do uso de classes POJO.
- Criamos dados iniciais através do uso de classe Data Factory, pra facilitar a criação e controle dos mesmos.
- Nesse projeto fazemos o uso do JUnit 5, que nos dá a possibilidade de usar a anotação DisplayName para dar descrições em português para nossos testes.


