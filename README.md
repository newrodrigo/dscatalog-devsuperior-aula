# DS Catalog
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/newrodrigo/dscatalog-devsuperior-aula/blob/main/LICENSE)

## Sobre o projeto
O DS Catalog é o resultado da construção de um backend durante o Bootcamp Java Spring da [DevSuperior](https://devsuperior.com.br/).

Principais características do projeto:
- Sistema de gerenciamento de catálogo de produtos com três níveis de acesso:
  - Visualização para usuários não autenticados
  - Adição de categorias/produtos para operadores
  - Administração de usuários para administradores
- Inclusão de testes Junit para garantir a robustez do sistema, simplificando a exploração e administração do catálogo de produtos.

Tópicos abordados no projeto:
- Implementação de Continuous Integration/Continuous Deployment (CI/CD)
- Implantação utilizando Docker, AWS, Heroku e Railway, proporcionando uma experiência completa de desenvolvimento e implantação do sistema de catálogo em diferentes plataformas.

## Documentação da API
A documentação detalhada da API pode ser encontrada no Postman:
[Visualizar Documentação no Postman](https://documenter.getpostman.com/view/21069954/2s9Xy2NBqS)

## Exemplos de consultas realizadas no Postman
1. **Realizar autenticação:**
   - Método: POST
   - Endpoint: `/oauth/token`
     ![Autenticação](https://github.com/newrodrigo/dscatalog-devsuperior-aula/assets/88519491/b53197b2-441b-4467-a65f-2c001738d763)

2. **Listar categorias paginadas:**
   - Método: GET
   - Endpoint: `/categories`
    ![Listagem de Categorias](https://github.com/newrodrigo/dscatalog-devsuperior-aula/assets/88519491/5a715da3-66a6-496b-aa76-d77d6087802b)

3. **Buscar produto por ID:**
   - Método: GET
   - Endpoint: `/products/2`
     ![Produto por ID](https://github.com/newrodrigo/dscatalog-devsuperior-aula/assets/88519491/117182e9-7801-40fb-bbd9-5cf146e29ffd)

4. **Inserir um novo produto:**
   - Permite inserir um novo produto, com validações de preço positivo e requisitos para o campo "name".
   - Método: POST
   - Endpoint: `/products`
     ![PostProducts](https://github.com/newrodrigo/dscatalog-devsuperior-aula/assets/88519491/e462ebb8-dda7-4533-bcb2-2d6c21ece942)
     ![PostProducts](https://github.com/newrodrigo/dscatalog-devsuperior-aula/assets/88519491/ed923778-b07d-4a60-bd07-25b9025966c5)

5. **Cadastrar novo usuário:**
   - Método: POST
   - Endpoint: `/users`
     ![NewUser](https://github.com/newrodrigo/dscatalog-devsuperior-aula/assets/88519491/73ee8b10-d7a8-4dcd-b4e0-df012b08e405)

## Modelo conceitual
![Modelo Conceitual](https://github.com/newrodrigo/dscatalog-devsuperior-aula/assets/88519491/a5e4299c-8eef-483f-bec3-2edff65f1efb)

# Tecnologias utilizadas
## Back end
- Java
- Spring Boot
- JPA / Hibernate
- SQL
- Maven
- OAuth/JWT
- Junit
- H2
- Postgres

## Implantação em produção
- Back end: Railway
- Banco de dados: Postgresql

# Como executar o projeto
## Back end
Pré-requisitos: Java 11

```bash
# Clonar o repositório
git clone git@github.com:newrodrigo/dscatalog-devsuperior-aula.git

# Acessar a pasta do projeto back end
cd backend

# Executar o projeto
./mvnw spring-boot:run
```

# Autor
Rodrigo Oliveira Cerqueira

[LinkedIn](https://www.linkedin.com/in/rodrigooc)
