# Aplicação To Do List

Criação de uma aplicação web service para To Do List em Java, utilizando a framework Springboot. A aplicação foi criada durante a Semana de Java criada pela empresa Rocketseat em outubro de 2023.

### Utilização da aplicação

Para consumo e acesso da aplicação, é recomendado o uso de apps como o API Dog, Thunder Client, Postman, dentre outros.

## Endpoints

#### Cadastro de Usuário -> POST https://todolist-javaspring-rocket.onrender.com/users/
``` json
{
  "name": "Nome Do Usuário",
  "username": "nomedousuario",
  "password": "12345"
}
```

#### Cadastro de Tarefas -> POST https://todolist-javaspring-rocket.onrender.com/tasks/
``` json
{
  "description":"Descrição da Tarefa",
  "title": "Título da Tarefa",
  "priority": "Nível de prioridade - ALTA, MÉDIA, BAIXA",
  "startAt": "2023-10-19T12:30:00",
  "endAt": "2023-10-19T15:35:00",
}
```
- Para cadastrar tarefas, é necessário fazer primeiramente o cadastro do usuário.
- Para a autenticação, deve-se utilizar o username e o password feitos no cadastro de usuário.

#### Pesquisa de Tarefas -> GET https://todolist-javaspring-rocket.onrender.com/tasks/
- A pesquisa de tarefas é feita para conferência de tarefas cadastradas por usuários autenticados.
- Para a pesquisa, deve-se fazer a autenticação do usuário, utilizando o username e o password feitos no cadastro de usuário.

#### Atualização de Tarefas -> PUT https://todolist-javaspring-rocket.onrender.com/tasks/ID-da-tarefa
- A atualização só pode ser feitos por usuário cadastrados.
- O usuário cadastrado não poderá alterar as tarefas criadas por outros usuários.
- Para acessar a tarefa a ser atualizada, deve-se inserir na URL o ID da tarefa, gerado no Cadastro de Tarefas.
- Para a atualização, deve-se fazer a autenticação do usuário, utilizando o username e o password feitos no cadastro de usuário.
  

## Deploy

URL: https://todolist-javaspring-rocket.onrender.com 

## Tecnologias utilizadas

- Java 17
- Spring Boot
- Maven
- H2 Database
- Bcrypt
- Lombok

## Contato

- Github: (https://github.com/lucasfierce)
- Linkedin: (https://www.linkedin.com/in/lucas-santos-527a30174/)
