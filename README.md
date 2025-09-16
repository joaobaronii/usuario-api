# Cadastro de Usuários - Spring Boot

Este projeto é uma API REST desenvolvida com **Spring Boot** para realizar operações de CRUD de usuários.  
A aplicação utiliza **Spring Data JPA** para persistência no banco de dados **PostgreSQL**.

## Funcionalidades

- **Criar Usuário** (`POST /usuario`)
- **Buscar Usuário por Email** (`GET /usuario?email={email}`)
- **Deletar Usuário por Email** (`DELETE /usuario?email={email}`)
- **Atualizar Usuário por ID** (`PUT /usuario?id={id}`)

## Tecnologias Utilizadas

- **Java 17+**
- **Spring Boot**
- **Spring Web**
- **Spring Data JPA**
- **PostgreSQL**
- **Lombok**

## Estrutura do Projeto

src/main/java/com/jbaroni/cadastrousuarios
├── CadastrousuariosApplication.java 
├── controller
│ └── UsuarioController.java 
├── service
│ └── UsuarioService.java 
├── entitys
│ └── Usuario.java 
└── repository
└── UsuarioRepository.java

## Configuração do Banco de Dados

O arquivo `application.properties` já está configurado para PostgreSQL:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/cadastrosusuario
spring.datasource.username=postgres
spring.datasource.password=0710
spring.jpa.hibernate.ddl-auto=update
```
