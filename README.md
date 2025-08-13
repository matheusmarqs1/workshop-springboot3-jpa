# 📦 API de Vendas - Projeto Acadêmico

API REST para um sistema de vendas, com operações de gerenciamento para usuários, produtos, pedidos e categorias.
Desenvolvida em Java com Spring Boot, aplicando boas práticas e arquitetura REST.

> **Diferencial:** além das práticas do curso "Workshop Spring Boot 3 + JPA" do Nélio Alves, realizei deploy no **Render** utilizando **Docker** e banco **PostgreSQL** gerenciado na nuvem, com configuração via variáveis de ambiente.

---

## 🚀 Tecnologias Utilizadas

-   **Backend:** Java 21, Spring Boot 3, Spring Data JPA
-   **Banco de dados:** PostgreSQL (produção), H2 Database (testes)
-   **DevOps:** Docker, Render
-   **Ferramentas:** Maven, Git, Postman

---

## ✨ Funcionalidades

Com base na implementação do código, as seguintes funcionalidades estão disponíveis nos endpoints:

* **Usuários:** CRUD completo (Criação, Leitura, Atualização e Deleção)
* **Produtos:** Leitura de todos os produtos e de produtos por ID
* **Pedidos:** Leitura de todos os pedidos e de pedidos por ID
* **Categorias:** Leitura de todas as categorias e de categorias por ID
* **Itens de Pedido:** Detalhes de cada pedido (implementado dentro da entidade de `Pedidos`)

---

## 🌐 Deploy

-   Plataforma: **Render**
-   Containerização: **Docker**
-   Banco: PostgreSQL gerenciado

🔗 **API em Produção:** [https://springcourse-render.onrender.com](https://springcourse-render.onrender.com)
*Obs.: Esta API retorna dados no formato **JSON**. Para visualizar melhor, utilize ferramentas como Postman ou acesse endpoints específicos, como `/users`.*

---

## 💻 Como Executar

### Com Docker

1.  **Construa a imagem Docker:**
    ```bash
    docker build -t api-vendas .
    ```
2.  **Execute o container:**
    ```bash
    docker run -p 8080:8080 api-vendas
    ```
    Acesse a API em: `http://localhost:8080`

### Sem Docker

1.  **Pré-requisitos:**
    * Instale Java 21 e PostgreSQL localmente.
    * Configure o arquivo `application.properties`.
2.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/matheusmarqs1/workshop-springboot3-jpa.git](https://github.com/matheusmarqs1/workshop-springboot3-jpa.git)
    ```
3.  Importe o projeto na sua IDE e execute a classe `CourseApplication.java`.

### 📄 Endpoints Principais

| Método | Endpoint | Descrição |
| :--- | :--- | :--- |
| `GET` | `/users` | Lista todos os usuários |
| `GET` | `/users/{id}` | Busca um usuário por ID |
| `POST` | `/users` | Cria um novo usuário |
| `PUT` | `/users/{id}` | Atualiza um usuário existente |
| `DELETE` | `/users/{id}` | Remove um usuário |

---

### 🧠 O que aprendi com este projeto

Este projeto foi fundamental para solidificar meu entendimento sobre o desenvolvimento backend e a arquitetura de APIs REST. Através dele, pude:

* **Aplicar conceitos de POO (Programação Orientada a Objetos):** Implementar classes, herança, encapsulamento e polimorfismo para criar um código mais organizado e reutilizável.
* **Dominar o ecossistema Spring Boot:** Utilizar injeção de dependências, anotações e o framework Spring Data JPA para criar uma aplicação robusta de forma ágil.
* **Trabalhar com persistência de dados:** Conectar a aplicação a bancos de dados relacionais (PostgreSQL e H2), entendendo o ciclo de vida das entidades e as operações de CRUD.
* **Praticar boas práticas de código:** Escrever um código limpo, documentado e com arquitetura em camadas (Controllers, Services, Repositories).
* **Compreender o processo de deploy:** Containerizar a aplicação com Docker e realizar o deploy em uma plataforma de nuvem (Render), conectando a um banco de dados externo.

### 📝 Conclusão

Este projeto representa não apenas a aplicação de conhecimentos técnicos, mas também a minha jornada de aprendizado e aprofundamento na área de desenvolvimento backend. A experiência de criar uma API completa, desde o desenvolvimento local até o deploy em produção, reforçou meu interesse por essa área e me preparou para novos desafios.
