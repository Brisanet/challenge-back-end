## Desafio Back end Brisalabs :computer:

- O desafio consiste no desenvolvimento de uma API REST utilizando as tecnologias listadas abaixo.
- Caso não termine desenvolver todo o desafio, envia o que conseguir que nós avaliaremos com muito prazer.
- Crie um repositório público no GitHub e envie o link para o e-mail `vanericadias@grupobrisanet.com.br` com assunto `Desafio Back end Brisalabs`.

## Tecnologias :rocket:

  - [NestJS](https://nestjs.com/) ou [Express](https://expressjs.com/pt-br/)
  - [Typescript](https://www.typescriptlang.org/)
  - [Typeorm](https://typeorm.io/#/)
  - [Postgres](https://www.postgresql.org/)
  - [Insomnia](https://insomnia.rest/)
  - REST

## Sobre o desafio :pushpin:
- O desafio consiste em desenvolver uma API REST para o sistema de transações do BrisaPIX.

- **Básico**
  - Requisitos
    - O sistema deve ser capaz de estabelecar uma conexão com um banco de dados Postgres.
    - O sistema deve ser capaz de lidar com requisições com formato de dados do tipo `JSON`.
    - O sistema deve ser capaz de cadastrar usuários.
    - O sistema deve ser capaz de persistir essas informações em um banco de dados relacional.
  - Adicionar arquivo de rotas do Insomnia 
  - Adicionar migrations

- **Intermediário**
  - Requisitos
    - O sistema deve ser capaz de cadastrar chaves PIX para os usuários já cadastrados.
    - Uma chave não poderá ser cadastrada mais de uma vez.
    - Cada usuário poderá ter no máximo 3 chaves.
    - O sistema deve ser capaz de realizar transações PIX utilizando chaves cadastradas de usuários.
    - Cada transação deve ser identificada de forma única por um id.
    - Cada transação deve conter a chave do usuário que envia e do usuário que recebe o PIX, além do valor, claro.
    - O sistema deve ser capaz de persistir essas informações em um banco de dados relacional.
  - Adicionar testes unitários 

- **Avançado**
  - Requisitos
    - O sistema deve ser capaz de enviar um email notificando o envio e recebimento de um pix.
    - O email de chegada deve ter o valor recebido, o nome de quem enviou e a data.
    - O email de envio deve ter o valor enviado, o nome de quem recebeu e a data.
  - Adicionar tratamento de erros de maneira global

- **Bonus**
  - Adicionar um `docker-compose` e um `Dockerfile`.
  - Adicionar o diagrama do banco de dados.

## Entidades :pencil2:
  - Usuários
    - O usuário deve possuir nome (nome do usuário), telefone (telefone do usuário), email e um id.
  - Chaves.
    - A entidade chaves deve possuir um valor (referente a chave a ser salva), id e a relação com o usuário dono da chave.
  - Transações.
    - A transação deve possuir um valor (referente ao valor em R$ da transação), relação com quem envia e quem recebe o PIX (usuário que envia e usuário que recebe o PIX) e um id.

## Critérios de avaliação :memo:
- Arquitetura
- Clean code
- Clareza
- Ausência de bugs
