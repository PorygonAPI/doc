<h1 align="center">Preparação dos Ambientes - Porygon3</h1>

<h1 align="center">Sumário</h1>

<p align="center">
  <a href ="#descrição-do-projeto"> DESCRIÇÃO DO PROJETO </a>  •
  <a href ="#requisitos"> REQUISITOS </a>  •
  <a href ="#configuração-do-banco-de-dados"> CONFIGURAÇÃO DO BANCO DE DADOS </a>  •
  <a href="#configuração-server"> CONFIGURAÇÃO SERVER </a> •
  <a href="#configuração-client"> CONFIGURAÇÃO CLIENT </a>
</p>

# DESCRIÇÃO DO PROJETO

O Porygon3 é uma aplicação web acadêmica que segue os princípios de desenvolvimento ágil com Scrum. O projeto está organizado em três repositórios principais:
- **Server**: Implementa o backend usando Java e Spring Boot, com operações RESTful e integra o banco de dados MySQL.
- **Client**: Responsável pelo front-end da aplicação, constrói a interface do usuário com foco na experiência e design.
- **Doc**: Armazena a documentação do projeto, como burndown, arquivos de teste, contribuição e backlogs.


## REQUISITOS

Para que possa testar a aplicação, é necessário que baixe e configure as ferramentas e extensões nas versões abaixo:

- **Java 22**
- **Spring Boot 3.3.3**
- **Maven** para gerenciamento de dependências
  - Spring Data JPA
  - Spring Web
  - Spring DevTools
- **MySQL** configurado e rodando
- **Docker**
- **Vue 3**

## CONFIGURAÇÃO DO BANCO DE DADOS

1. Certifique-se de que o MySQL está instalado e em execução.
2. Crie um banco de dados chamado `porygon`.
    ```sql
    create database porygon
    ```

3. Copie e cole o `schema.sql` e o `data.sql` presentes no repositório `server` na aba de Query no MySQL, nesta ordem, para criar as tabelas e popular o banco.

## CONFIGURAÇÃO SERVER

1. Clone o repositório para o seu ambiente local:

    ```bash
    git clone https://github.com/PorygonAPI/server.git
    ```

2. Navegue até o diretório do projeto e abra na IDE da sua escolha:

    ```bash
    cd PorygonAPI/server
    ```

3. Execute o comando Maven no terminal da sua IDE para construir o projeto:

    ```bash
    mvn clean install
    ```

4. Configure o arquivo `application.properties` no repositório `server` para incluir as informações de conexão com o banco de dados:

    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/porygon?useSSL=false&serverTimezone=UTC&allowPublicKeyRetrieval=true
    spring.datasource.username=seu_usuario
    spring.datasource.password=sua_senha
    spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
    ```

5. Execute o comando abaixo no terminal ou clique em `Run Java` no arquivo `PorygonApplication`

    ```bash
    mvn spring-boot:run
    ```

## CONFIGURAÇÃO CLIENT

1. Clone o repositório para o seu ambiente local:

    ```bash
    git clone https://github.com/PorygonAPI/client.git
    ```

2. Navegue até o diretório do projeto e abra na IDE da sua escolha:

    ```bash
    cd PorygonAPI/client
    ```

3. Execute o comando abaixo no terminal da sua IDE para construir o projeto:

    ```bash
    npm install
    ```

4. Execute o comando abaixo no terminal da sua IDE para subir a aplicação e cole a URL que aparecer (`http://localhost:5173/`):

    ```bash
    npm run dev
    ```

