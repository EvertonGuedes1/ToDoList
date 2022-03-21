# ToDoList

## Criar Usuário

- Método: `PUT`
- Path: `/user`
- Body:
  - `name` (obrigatório)
  - `nickname` (obrigatório)
  - `email` (obrigatório)

## Pegar Usuário Pelo id

- Método: `GET`
- Path: `/user/:id`
- Body de resposta (retornar um erro se não encontrar):
  - `id`
  - `nickname`

## Editar Usuário

- Método: `POST`
- Path: `/user/edit/:id`
- Body:
  - `name` (opcional, não pode ser vazio)
  - `nickname` (opcional, não pode ser vazio)
  - `email` (opcional, não pode ser vazio)

## Criar Tarefa

- Método: `PUT`
- Path: `/task`
- Body:
  - `title` (obrigatório)
  - `description` (obrigatório)
  - `deadline` (obrigatório, formato DD/MM/YYYY)
  - `authorid`

## Pegar Tarefa Pelo id

- Método: `GET`
- Path: `/task/:id`
- Body de resposta (retornar um erro se não encontrar):
  - `id`
  - `title`
  - `description`
  - `deadline` (formato DD/MM/YYYY)
  - `status`
  - `authorind`
  - `authorNickname`
