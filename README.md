# Node API-SOLID

## 💻 Projeto

**[Node API-SOLID](https://github.com/AdrianoTobias/node-api-solid)**, é uma aplicação que segue o estilo do "Wellhub (GymPass)". Seu desenvolvimento é voltado à utilização de Design Patterns, princípios do SOLID e testes automatizados. Para isso, o projeto engloba a construção de API's REST, testes unitários e end-to-end, além de integração e deploy contínuos.

A aplicação visa os seguintes requisitos:

### Requisitos funcionais (RF)

- [x] Deve ser possível se cadastrar;
- [x] Deve ser possível se autenticar;
- [x] Deve ser possível obter o perfil de um usuário logado;
- [x] Deve ser possível obter o número de check-ins realizados pelo usuário logado;
- [x] Deve ser possível o usuário obter o seu histórico de check-ins;
- [x] Deve ser possível o usuário buscar academias próximas (até 10km);
- [x] Deve ser possível o usuário buscar academias pelo nome;
- [x] Deve ser possível o usuário realizar check-in em uma academia;
- [x] Deve ser possível validar o check-in de um usuário;
- [x] Deve ser possível cadastrar uma academia;

### Regras de negócio (RN)

- [x] O usuário não deve poder se cadastrar com um e-mail duplicado;
- [x] O usuário não pode fazer 2 check-ins no mesmo dia;
- [x] O usuário não pode fazer check-in se não estiver perto (100m) da academia;
- [x] O check-in só pode ser validado até 20 minutos após ser criado;
- [x] O check-in só pode ser validado por administradores;
- [x] A academia só pode ser cadastrada por administradores;

### Requisitos não-funcionais (RNF)

- [x] A senha do usuário precisa estar criptografada;
- [x] Os dados da aplicação precisam estar persistidos em um banco PostgreSQL;
- [x] Todas listas de dados precisam estar paginadas com 20 itens por página;
- [x] O usuário deve ser identificado por um JWT (JSON Web Token);


É uma aplicação desenvolvida durante o **[MBA Fullstack](https://www.rocketseat.com.br/mba)**, provido pela **[Rocketseat](https://rocketseat.com.br/)**, em parceria com a **[Sirius Education](https://landing.sirius.education/home/)**.


## 🧪 Tecnologias

Esse projeto foi desenvolvido com as seguintes tecnologias:

- [Node.js](https://nodejs.org/)
- [TypeScript](https://www.typescriptlang.org/)
- [Fastify](https://fastify.dev/)
- [Prisma](https://www.prisma.io/)
- [Zod](https://github.com/colinhacks/zod)
- [Vitest](https://vitest.dev/)


## 🚀 Como executar

Clonar o projeto e acessar a pasta do mesmo:

```bash
$ git clone https://github.com/AdrianoTobias/node-api-solid.git
$ cd node-api-solid
```

Para iniciá-lo:
```bash
# Instalar as dependências
$ npm install
```

> Esse projeto depende do [Docker](https://docs.docker.com/get-started/get-docker/) para rodar o banco de dados. Após tê-lo instalado:

```bash
# Criar o container
$ docker compose up -d

# Criar a estrutura do banco de dados
$ npm run pretest:e2e
```

```bash
# Iniciar a aplicação
$ npm run start:dev
```
A aplicação estará disponível no endereço http://localhost:3333.

Para executar os testes:
```bash
# Iniciar os testes unitários
$ npm run test

# Iniciar os testes end-to-end
$ npm run test:e2e
```



[Adriano Tobias](https://github.com/AdrianoTobias)