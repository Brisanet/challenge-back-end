## Desafio Back end Brisalabs :computer:

- O desafio consiste no desenvolvimento de uma API REST utilizando as tecnologias listadas abaixo.
- Caso não termine desenvolver todo o desafio, envie o que conseguir que nós avaliaremos com muito prazer.
- Crie um repositório público no GitHub e envie o link para o e-mail `vanericadias@grupobrisanet.com.br` com assunto `Desafio Back end Brisalabs`.

## Tecnologias :rocket:

- [NestJS](https://nestjs.com/) ou [Express](https://expressjs.com/pt-br/)
- [Typescript](https://www.typescriptlang.org/)
- [Prisma](https://www.prisma.io/)
- [Postgres](https://www.postgresql.org/)
- [Insomnia](https://insomnia.rest/)
- [Jest](https://jestjs.io) ou [Vitest](https://vitest.dev)
- [Zod](https://github.com/colinhacks/zod) ou [Joi](https://joi.dev) ou [Celebrate](https://github.com/arb/celebrate)
- [Docker](https://www.docker.com)
- REST

## Sobre o desafio :pushpin:

- O desafio consiste em desenvolver uma API REST para o sistema de BrisaAcademic.

- **Básico**

  - Requisitos
    - O sistema deve ser capaz de estabelecer uma conexão com um banco de dados Postgres.
    - O sistema deve ser capaz de lidar com requisições com formato de dados do tipo `JSON`.
    - O sistema deve ser capaz de cadastrar professores, alunos e cadeiras(matérias).
    - O sistema deve ser capaz de persistir essas informações em um banco de dados relacional.
  - Adicionar arquivo de rotas do Insomnia
  - Adicionar migrations
  - Adicionar o diagrama do banco de dados

- **Intermediário**

  - Requisitos
    - O professor deve ser capaz de cadastrar uma ou mais cadeiras(matérias).
    - O aluno deve ser capaz de se matricular em uma ou mais cadeiras(matérias).
    - O professor deve assentir as solicitações de matrículas dos alunos.
    - Uma cadeira não poderá ser ofertada mais de uma vez por período.
    - Um aluno não pode se matricular em mais de 8 cadeiras(matérias) e menos de 1.
    - O sistema deve ser capaz de listar todas as cadeiras e seus alunos matriculados.
    - O sistema deve possuir dois módulos "aluno e professor". Dica: pode ser utilizado o [JWT](https://jwt.io/).
    - O sistema deve ser capaz de persistir essas informações em um banco de dados relacional.
  - Adicionar testes unitários

- **Avançado**

  - Requisitos
    - O sistema deve ser capaz de enviar um email notificando o aluno que a matricula de determinada cadeira(matéria) foi bem sucedida.
    - O email deve conter o nome da cadeira e o nome do professor.
  - Adicionar tratamento de erros de maneira global
  - Adicionar um `docker-compose` e um `Dockerfile`

- **Bonus**
  - Adicionar teste de ponta a ponta(E2E)
  - [Swagger](https://swagger.io)

## Entidades :pencil2:

- Professor
  - A entidade deve possuir nome, telefone, email, CPF e um id.
- Aluno.
  - A entidade deve possuir nome, telefone, email, CPF, matrícula e um id.
- Cadeira.
  - A entidade deve conter nome, slug, data de inicio e data de fim(período de disponibilidade), carga horaria, o id do professor que a criou e um id.
- Cadeiras dos alunos
  - A entidade deve possuir o id do aluno, o id da cadeira e seu próprio id.

## Critérios de avaliação :memo:

- Arquitetura
- Clean code
- Clareza
- Ausência de bugs
- Validação de dados
