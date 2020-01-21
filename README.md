# DevRadar ( Backend - Semana Omnistack 10 / Rocketseat )

## Getting Started

Estas instruções permitirão copiar o projeto e rodá-lo localmente para propósito de testes e desenvolvimento.

### Pré-requisitos

- [Node.js](https://nodejs.org/en/)
- [Yarn](https://yarnpkg.com/lang/en/) ou [NPM](https://www.npmjs.com/get-npm)
- [MongoDB](https://www.mongodb.com/)

## Backend

- Estruturação da API do projeto
- Sistemática de requisição e resposta
- Parâmetros em API
  - Query Params: request.query(filtros, ordenação, paginação)
  - Route Params: request.params(identificar um recurso na alteração ou remoção)
  - Body: request.body(dados para criação ou alteração de registros)
- Funcionalidades
  - Criar um novo dev: POST /dev
  - Pesquisar um novo dev: GET /search
  - Listar todos os devs: GET /index
- Dependências
  - "axios": "^0.19.1",
  - "cors": "^2.8.5",
  - "express": "^4.17.1",
  - "mongoose": "^5.8.7",
  - "socket.io": "^2.3.0"
- Softwares
  - Insomnia
  - MongoDB Compass
  - MongoDB Atlas

### Início

#### Clonar o repositório

Inserir o comando a baixo na pasta desejada para salvar o projeto.

`git clone [link do repositório]`

## Conectar ao banco de dados

- Deve-se acessar o MongoDB através do site e logar em sua conta.
- Após configurar o Cluster copiar o link fornecido pelo MongoDB para conexão e substituir no arquivo 'index.js' conforme a baixo.

`mongoose.connect('Link de conexão com o Mongo', {
  useNewUrlParser: true,
  useUnifiedTopology: true
});`
