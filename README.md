# Desafio CRUD de Clientes

API REST desenvolvida como desafio do curso **Java Spring Professional** da [DevSuperior](https://devsuperior.com.br), implementando um CRUD completo com tratamento de exceções e validação de dados.

## Sobre o projeto

Sistema para gerenciamento de clientes com as cinco operações básicas de uma API REST. O projeto inclui tratamento de erros customizado e validação de dados com Bean Validation.

## Modelo de domínio

**Client:** `id`, `name`, `cpf`, `income`, `birthDate`, `children`

## Tecnologias utilizadas

- Java 21
- Spring Boot 3
- Spring Data JPA
- Bean Validation
- H2 Database
- Maven

## Endpoints

| Método | Rota | Descrição |
|---|---|---|
| GET | `/clients` | Listagem paginada de clientes |
| GET | `/clients/{id}` | Busca cliente por ID |
| POST | `/clients` | Insere novo cliente |
| PUT | `/clients/{id}` | Atualiza cliente |
| DELETE | `/clients/{id}` | Deleta cliente |

## Tratamento de erros

| Situação | Status HTTP |
|---|---|
| ID não encontrado (GET, PUT, DELETE) | 404 Not Found |
| Dados inválidos (POST, PUT) | 422 Unprocessable Entity |

## Como executar

```bash
git clone https://github.com/pedrotrevisan/desafio-crud-clientes.git
cd desafio-crud-clientes
./mvnw spring-boot:run
```

H2 Console: `http://localhost:8080/h2-console`

## Autor

**Pedro Henrique Trevisan**

[![GitHub](https://img.shields.io/badge/GitHub-pedrotrevisan-black)](https://github.com/pedrotrevisan)
