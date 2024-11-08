# Controle de Bookcases

## Descrição
Este projeto é uma API para gerenciar bookcases (estantes de livros). Ele permite operações CRUD (Criar, Ler, Atualizar e Deletar) para bookcases.

## Estrutura do Projeto
O projeto é construído em Ruby on Rails e segue a arquitetura MVC (Model-View-Controller).

## Controlador: `BookcasesController`

### Rotas
As seguintes rotas estão disponíveis para o controlador de bookcases:

- `GET /bookcases` - Retorna uma lista de todas as bookcases.
- `GET /bookcases/:id` - Retorna uma bookcase específica pelo ID.
- `POST /bookcases` - Cria uma nova bookcase.
- `PATCH/PUT /bookcases/:id` - Atualiza uma bookcase existente.
- `DELETE /bookcases/:id` - Deleta uma bookcase existente.

### Métodos

#### `index`
- **Descrição**: Retorna todas as bookcases.
- **Resposta**: JSON com a lista de bookcases.

#### `show`
- **Descrição**: Retorna uma bookcase específica.
- **Parâmetros**: `id` da bookcase.
- **Resposta**: JSON com os detalhes da bookcase.

#### `create`
- **Descrição**: Cria uma nova bookcase.
- **Parâmetros**: `bookcase` com os atributos permitidos.
- **Resposta**: JSON com a bookcase criada ou erros de validação.

#### `update`
- **Descrição**: Atualiza uma bookcase existente.
- **Parâmetros**: `id` da bookcase e `bookcase` com os atributos permitidos.
- **Resposta**: JSON com a bookcase atualizada ou erros de validação.

#### `destroy`
- **Descrição**: Deleta uma bookcase existente.
- **Parâmetros**: `id` da bookcase.
- **Resposta**: Nenhuma (204 No Content).


