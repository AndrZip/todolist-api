# API Todolist

<p align="center">
  <img src="https://i.pinimg.com/originals/a2/4c/b5/a24cb568fa40046f8562dbc45cea8506.gif" alt="Imagem da API">
</p>

A API Todolist é uma aplicação simples para gerenciar listas de tarefas (to-do lists). Ela permite que os usuários criem, atualizem, excluam e visualizem suas listas de tarefas de forma eficiente.

## Índice

1. [Requisitos](#requisitos)
2. [Instalação](#instalação)
3. [Uso](#uso)
4. [Endpoints](#endpoints)
5. [Exemplos](#exemplos)
6. [Contribuição](#contribuição)
7. [Licença](#licença)

## Requisitos

Antes de começar a usar a API, certifique-se de que você tenha as seguintes dependências instaladas:

- Node.js
- npm ou Yarn
- Banco de dados (por exemplo, MongoDB)

## Instalação

Siga estas etapas para instalar e configurar a API Todolist:

1. **Clone este repositório:**

   ```bash
   git clone https://github.com/seu-usuario/todolist-api.git
   ```

2. **Navegue até o diretório da API:**

   ```bash
   cd todolist-api
   ```

3. **Instale as dependências:**

   ```bash
   npm install
   # ou
   yarn install
   ```

4. **Configure as variáveis de ambiente.** Crie um arquivo `.env` na raiz do projeto e defina as seguintes variáveis:

   ```dotenv
   PORT=3000
   MONGODB_URI=sua_url_de_conexão_com_o_banco_de_dados
   ```

5. **Inicie o servidor:**

   ```bash
   npm start
   # ou
   yarn start
   ```

   A API estará disponível em `http://localhost:3000` por padrão.

## Uso

A API Todolist é simples de usar e possui endpoints bem definidos para gerenciar suas listas de tarefas. Você pode acessar os endpoints usando métodos HTTP como GET, POST, PUT e DELETE.

## Endpoints

Aqui estão os principais endpoints da API:

- `GET /tasks`: Retorna todas as tarefas.
- `GET /tasks/:id`: Retorna uma tarefa específica pelo ID.
- `POST /tasks`: Cria uma nova tarefa.
- `PUT /tasks/:id`: Atualiza uma tarefa existente pelo ID.
- `DELETE /tasks/:id`: Exclui uma tarefa pelo ID.

Consulte a documentação completa da API para obter detalhes sobre como usar esses endpoints.

## Exemplos

Aqui estão alguns exemplos de como usar a API:

### Criar uma nova tarefa

```bash
curl -X POST http://localhost:3000/tasks -H "Content-Type: application/json" -d '{"title": "Comprar leite"}'
```

### Atualizar uma tarefa

```bash
curl -X PUT http://localhost:3000/tasks/1 -H "Content-Type: application/json" -d '{"title": Comprar cereal, "status": "finalizado"}'
```

## Contribuição

Contribuições são bem-vindas! Se você quiser contribuir para a API Todolist, siga estas etapas:

1. **Fork este repositório.**
2. **Crie uma branch para sua contribuição:** `git checkout -b feature/nova-funcionalidade`.
3. **Faça suas alterações e commit.**
4. **Push para o seu fork:** `git push origin feature/nova-funcionalidade`.
5. **Crie um pull request neste repositório.**

## Licença

Este projeto está licenciado sob a Licença MIT. Consulte o arquivo [LICENSE](LICENSE) para obter detalhes.

---
