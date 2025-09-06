# CRUD Básico em Java ☕️

![Java](https://img.shields.io/badge/Java-17+-red?style=for-the-badge&logo=openjdk)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3-green?style=for-the-badge&logo=springboot)
![Maven](https://img.shields.io/badge/Maven-3-blue?style=for-the-badge&logo=apachemaven)

Um projeto simples de **CRUD (Create, Read, Update, Delete)** desenvolvido em **Java com Spring Boot**.  
O objetivo é servir como **base de estudo** para quem deseja aprender a criar **APIs REST**, aplicar boas práticas e trabalhar com **Spring Data JPA**.

---

## 🚀 Tecnologias utilizadas
- **Java 17+**
- **Spring Boot**
- **Spring Web**
- **Spring Data JPA**
- **H2 Database** (para testes)
- **Maven**

---

## 📂 Estrutura do projeto
src/main/java/com/crudbasicojava/
├── controller # Endpoints da API REST
├── service # Camada de regras de negócio
├── repository # Comunicação com o banco via JPA
└── model # Entidades

yaml


---

## ⚙️ Funcionalidades
- Criar um novo usuário (`POST /usuario`)
- Buscar usuário por e-mail (`GET /usuario?email=...`)
- Atualizar usuário por ID (`PUT /usuario/{id}`)
- Deletar usuário por e-mail (`DELETE /usuario?email=...`)

---

## ▶️ Como executar o projeto

### Pré-requisitos
- **Java 17+**
- **Maven**

### Rodando localmente
```bash
# Clone este repositório
git clone https://github.com/elielfilhodev/crudbasicojava.git

# Acesse a pasta
cd crudbasicojava

# Compile e rode o projeto
mvn spring-boot:run
O projeto ficará disponível em:
👉 http://localhost:8080

📖 Exemplos de requisições
Criar usuário
http

POST /usuario
Content-Type: application/json

{
  "nome": "João Silva",
  "email": "joao@email.com",
  "cpf": "12345678900",
  "senha": "123456"
}
Buscar usuário por e-mail
http

GET /usuario?email=joao@email.com
Atualizar usuário por ID
http

PUT /usuario/{id}
Content-Type: application/json

{
  "nome": "João da Silva",
  "email": "joao.novo@email.com",
  "cpf": "12345678900",
  "senha": "novaSenha123"
}
Deletar usuário por e-mail
http

DELETE /usuario?email=joao@email.com
✅ Melhorias futuras
 Criar DTOs e adicionar Bean Validation

 Implementar tratamento global de exceções

 Adicionar paginação e filtros

 Criar testes unitários e de integração

 Documentar a API com Swagger (springdoc-openapi)

👨‍💻 Autor
Eliel Filho
