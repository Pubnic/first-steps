# Desafio

## Descrição
Criar uma API de Todo List onde eu consiga criar, listar todos, pegar um, editar e excluir.

## O que é preciso fazer?

### Todo precisa ter os seguintes atributos:
- title
- description
- status (TODO, DOING, DONE)
- due_date (Data para a entrega)
- responsible (Nome do responsável)

### Deverão ser implementado os seguintes endpoints:
- Listar todos os Todo
    - Retorna: uma lista contendo somente title e id
    - Método HTTP: GET
    - Endpoint: /todos
    - Status: 200
- Pegar um Todo
    - Retorna: um Todo com todos seus campos
    - Método HTTP: GET
    - Endpoint: /todos/id
    - Status: 200
- Criar um Todo
    - Retorna: o Todo criado com o ID
    - Método HTTP: POST
    - Endpoint: /todos
    - Status: 201
- Atualizar um Todo
    - Retorna: o Todo atualizado
    - Método HTTP: PUT
    - Endpoint: /todos/id
    - Status: 200
- Deletar um Todo
    - Retorna: Vazio
    - Método HTTP: DELETE
    - Endpoint: /todos/id
    - Status: 204

## Por onde começo?
- Antes de iniciar o desafio, certifique-se que configurou o seu ambiente de acordo com o [tutorial de backend na Wiki](wiki/environment/backend)
- Somente é necessário mexer nos seguintes arquivos
    - `todos/views.py`, onde você irá criar os endpoints.
    - `todos/db/models.py`, onde você irá adicionar os campos que faltam no Todo
- Para manipular o banco de dados, utilize a classe `TodosDBService` já importado em `todos/views.py`

Foi preparado um repositório com os requisitos mínimos para que você possa focar somente em aprender o framework FastAPI.
O repositório encontra-se no endereço [https://github.com/Pubnic/todo-challenge](https://github.com/Pubnic/todo-challenge) 

## Critério de conclusão
- Rodar o comando `flake8` no terminal e não retornar erros.
- Rodar o comando `pytest` no terminal e não retornar erros.

## Dúvidas?
- Olhe a documentação [https://fastapi.tiangolo.com/](https://fastapi.tiangolo.com/)
- Pergunte no canal do slack [#engineering](https://residnciapubnic.slack.com/archives/C024X1QGCMS)
