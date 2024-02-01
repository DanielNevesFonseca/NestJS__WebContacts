
# Documentação da API - WebContacts Backend

## 1. Visão Geral

Visão geral do projeto, um pouco das tecnologias usadas.

- [NodeJS](https://nodejs.org/en/)
- [NestJS](https://nestjs.com/)
- [TypeScript](https://www.typescriptlang.org/)
- [PostgreSQL](https://www.postgresql.org/)
- [TypeORM](https://typeorm.io/)
- [Docker](https://www.docker.com/)

A URL base da aplicação -  Rodando Localmente e DB em Docker:
http://localhost:3000

### Obs: A APLICAÇÃO RODA COM DB POSTGRESQL EM DOCKER(CONTAINER)


## 2. Início Rápido

### 2.1. Instalando Dependências e Iniciando projeto

2.1.1 - Clone o projeto em sua máquina e instale as dependências com o comando:

    $ npm install 

2.1.2 -(Docker Desktop instalado e rodando) - Criar o container docker e instanciá-lo - Rode os comando como adm( sudo - linux):
 
    $ docker compose up -d

2.1.3 - (Docker Desktop instalado e rodando) - Caso tenha problemas com path e o docker não reconheça o caminho do docker-compose.yml:

 1. Clique no ícone da engrenagem/Settings no canto superior direito;
 2. Clique na aba Resources/File Sharing;
 3. Adicione o caminho desse projeto clonado;
 
 2.1.4 - (Docker Desktop instalado e rodando) - Instancie o server do NestJS:

    $ npm run start

 
 Se tudo correr bem, o server do backend e a api estarão funcionando e poderá servir os services para o frontend!

A doc da API Rest está rodando na porta:
http://localhost:3000/docs

## 3. Observações

O próprio docker-compose e Dockerfile cuidam da criação de um usuário para o Database e variáveis de ambiente. Por esse motivo o .env está fora na base do repo.



