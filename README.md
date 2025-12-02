# - Node-express-cars

API simples criada com Node.js + Express para fins de estudo e prática de testes automatizados.
O objetivo do projeto é permitir a realização de operações CRUD (Create, Read, Update, Delete) sobre uma lista de carros armazenada em memória — sem banco de dados.

Este projeto também é utilizado para criar e praticar testes automatizados de API usando Cypress.

---

## - **Tecnologias utilizadas**

* **Node.js**
* **Express**
* **Nodemon**
* **JavaScript**
* **Cypress** (para testes automatizados)
* **Faker.js** (para gerar dados aleatórios nos testes)

##

---

## - Como rodar o projeto

### 1️⃣ Instale as dependências

```
npm install
```

### 2️⃣ Inicie o servidor

```
npm run dev
```

O servidor iniciará em:

```
http://localhost:3003
```

---

# - **Endpoints da API**

A API trabalha com o recurso **/cars**.

### ✔ **GET /cars**

Retorna a lista completa de carros.

### ✔ **GET /cars/**

Retorna apenas um carro específico pelo ID.

### ✔ **POST /cars**

Cria um novo carro.
Exemplo de requisição:

```json
{
  "nome": "Corolla XEi",
  "modelo": "XEi",
  "marca": "Toyota",
  "ano": 2020,
  "preco": 120000
}
```

### ✔ **PUT /cars/**

Atualiza um carro pelo ID.

### ✔ **DELETE /cars/**

Remove um carro da lista.

---

# - Testes automatizados com Cypress

Este projeto também conta com testes de API usando Cypress, incluindo:

* Criação de carro (POST)
* Busca de carro pelo ID (GET)
* Validação de status codes
* Uso de dados dinâmicos com Faker
* Chain de requisições (POST → GET)
* Verificação de estrutura do response

Exemplo de teste:

```js
it("Should create a car and get it back", () => {
    // POST
    // GET
    // Validations...
});
```

---

# - Objetivo do Projeto

Este projeto foi criado com foco em:

* Praticar Node.js e Express
* Estudar CRUD básico
* Criar uma API para treinar automação de testes
* Evoluir para um perfil SDET (Software Development Engineer in Test)

---

# - Próximos passos (Roadmap)

* Implementar integração com **MySQL** usando Sequelize ou Knex
* Criar camada de serviços (Service Layer)
* Adicionar validações mais robustas (Joi ou Zod)
* Criar testes de integração completos

---

# 🧑‍💻 Autor

**Nathanael Henrique Souza Nunes**
Foco em QA / SDET
Automação com Cypress | JavaScript | Node.js

---
