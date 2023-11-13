
# Nobuzz Challenge - Todo List

![demo screenshot](/screenshot.png)

Descrição

## Autores

- [@arturbacilla](https://www.github.com/arturbacilla)

## Tecnologias

<!-- Ícones tech: https://shields.io/  https://simpleicons.org/ -->
<!-- Basta descomentar cada tag para incluí-la no readme-->

**Linguagens:**  
 <picture>
  <source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/typescript-3178C6?style=for-the-badge&logo=typescript&logoColor=white">
  <img alt="Typescript" src="https://img.shields.io/badge/typescript-3178C6?style=for-the-badge&logo=typescript&logoColor=white">
</picture>

**Frontend:** 
 <picture>
  <source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/react-61DAFB?style=for-the-badge&logo=react&logoColor=black">
  <img alt="React" src="https://img.shields.io/badge/react-61DAFB?style=for-the-badge&logo=react&logoColor=black">
</picture>

**Backend:** 
 <picture>
  <source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white">
  <img alt="Node.js" src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white">
</picture>

 <picture>
  <source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/NestJS-ffffff?style=for-the-badge&logo=nestjs&logoColor=E0234E">
  <img alt="NestJS" src="https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=black">
</picture>

 <picture>
  <source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white">
  <img alt="Prisma" src="https://img.shields.io/badge/prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white">
</picture>

**Database:** 
 <picture>
  <source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/postgre-4169E1?style=for-the-badge&logo=postgresql&logoColor=black">
  <img alt="Postgre" src="https://img.shields.io/badge/postgre-4169E1?style=for-the-badge&logo=postgresql&logoColor=black">
</picture>

**Outros:** 
<picture>
  <source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/docker-2496ED?style=for-the-badge&logo=docker&logoColor=white">
  <img alt="Docker" src="https://img.shields.io/badge/docker-2496ED?style=for-the-badge&logo=docker&logoColor=black">
</picture>

<picture>
  <source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/jwt-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white">
  <img alt="JWT" src="https://img.shields.io/badge/jwt-ffffff?style=for-the-badge&logo=jsonwebtokens&logoColor=black">
</picture>

## Execução Local

Clone the project

```bash
  git clone git@github.com:arturbacilla/nobuzz-challenge.git
```

Go to the project directory

```bash
  cd ./nobuzz-challenge

```

#### Execução:

É necessario possuir o docker-engine (com docker compose) instalado para executar esse projeto.

<details>
<summary>
 <picture>
  <source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/linux-FCC624?style=for-the-badge&logo=linux&logoColor=black">
  <img alt="Linux" src="https://img.shields.io/badge/linux-FCC624?style=for-the-badge&logo=linux&logoColor=black">
</picture>
ou 
 <picture>
  <source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/apple-ffffff?style=for-the-badge&logo=apple&logoColor=white">
  <img alt="Apple" src="https://img.shields.io/badge/apple-ffffff?style=for-the-badge&logo=apple&logoColor=white">
</picture>
</summary>
Para usuários de linux (testado com ZSH e BASH) ou mac (não testado), executar o seguinte comando na pasta raiz do projeto e seguir as instruções: 

 ```bash
  ./nobuzz

```
 As vezes pode ser necessário permitir a execução do script com o comando:

 ```bash
  sudo chmod +x ./nobuzz
  
```
</details>

<details>
<summary>
 <picture>
  <source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/windows-0078D4?style=for-the-badge&logo=windows10&logoColor=white">
  <img alt="Windows" src="https://img.shields.io/badge/windows-0078D4?style=for-the-badge&logo=windows10&logoColor=white">
</picture>
</summary>
Se você é usuário de Windows e usa git-bash ou algum terminal padrão UNIX, seguir os passos das instruções de Linux/Mac.

Caso contrário, é necessário ter instalado o comando docker compose e alterar as variáveis de ambiente da seguinte forma:

#### Variáveis de ambiente

Renomeie o arquivo .env.example para .env localizado na raiz do projeto e insira as seguintes variáveis de ambiente (por exemplo):

`POSTGRES_PASSWORD=algumpassword`
`POSTGRES_USER=postgres`
`PGUSER=postgres`
`POSTGRES_DB=nobuzz_db`

Além disso, 
Renomear o arquivo ./app/backend/.env.example para ./app/backend/.env e inserir as variáveis de ambiente substituindo de acordo com as variáveis acima

`DATABASE_URL=postgresql://<$POSTGRES_USER>:<$POSTGRES_PASSWORD>@db:5432/ <$POSTGRES_DB>?schema=public`

Seguindo o exemplo acima ficaria desta forma:
`DATABASE_URL=postgresql://postgres:algumpassword@db:5432/nobuzz_db?schema=public`

`JWT_SECRET=algumsegredoJWT`

e por último executar na pasta raiz do projeto:
`docker compose up`
</details>

## Feedback

Se você tem algum feedback (que sempre são muito bem vindos!), visite meu perfil para pegar informações de contato.
