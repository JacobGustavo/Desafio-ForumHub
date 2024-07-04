# ForumHub

ForumHub é um projeto de API REST para gerenciamento de tópicos em um fórum, com operações CRUD para tópicos, cursos, respostas e usuários, além de autenticação de usuários utilizando Spring Security e tokens JWT. Este projeto foi desenvolvido como parte do desafio final do programa Alura ONE (Oracle Next Education) especialização em Back End.

## Funcionalidades

- **Autenticação de Usuários:** Login e cadastro de usuários com criptografia de senha e geração de tokens JWT.
- **Gerenciamento de Tópicos:** Criação, listagem, atualização de status e exclusão de tópicos.
- **Gerenciamento de Cursos:** Criação, listagem e exclusão de cursos.
- **Gerenciamento de Respostas:** Criação, listagem e exclusão de respostas para tópicos.
- **Documentação da API:** Utilização do Swagger para a documentação dos endpoints da API.

## Tecnologias Utilizadas

- Java 17
- Spring Boot 3
- Spring Security
- JWT
- Hibernate/JPA
- Jakarta Validation
- Swagger/OpenAPI 3

## Estrutura do Projeto

- **Controller:** Camada responsável por receber e processar as requisições HTTP.
- **Domain:** Entidades e serviços que representam as regras de negócio.
- **Infra:** Configurações de segurança e tratamento de exceções.
- **Repository:** Interfaces de persistência de dados.

## Como Executar

Clone o repositório:

```bash
git clone https://github.com/JacobGustavo/forumhub.git
cd forumhub
```

Application Properties:

```bash
spring.datasource.url=jdbc:mysql://localhost:3306/forumhub
spring.datasource.username=seu-usuario
spring.datasource.password=sua-senha
```

Execute o Projeto:

```bash
./mvnw spring-boot:run
```

Acesse a documentação da API:

```bash
http://localhost:8080/swagger-ui.html
```

# Endpoints Principais

## Autenticação

 - POST /login: Autenticação do usuário e geração do token JWT.
 
## Usuários
 
 - POST /usuario: Cadastro de um novo usuário.
 - GET /usuario: Listagem de todos os usuários.
 - PUT /usuario: Atualização de dados de um usuário.
 - DELETE /usuario/{id}: Exclusão de um usuário.

## Tópicos

 - POST /topico: Criação de um novo tópico.
 - GET /topico: Listagem de todos os tópicos.
 - PUT /topico/status: Atualização do status de um tópico.
 - DELETE /topico/{id}: Exclusão de um tópico.

## Cursos

 - POST /curso: Criação de um novo curso.
 - GET /curso: Listagem de todos os cursos.
 - DELETE /curso/{id}: Exclusão de um curso.

## Respostas
 - POST /resposta: Criação de uma nova resposta.
 - GET /resposta: Listagem de todas as respostas.
 - DELETE /resposta/{id}: Exclusão de uma resposta.


# Contato
 - Email: gustavo.hcj@hotmail.com
 - LinkedIn: [Gustavo Jacob](https://www.linkedin.com/in/gustavo-jacob-b6583a1aa)

## Badges Alura One
<img src="https://github.com/JacobGustavo/Desafio-ForumHub/assets/166851917/0c853f07-155a-472a-ba1e-048846fd9751" alt="Badge-Spring" width="200"/> <img src="https://github.com/JacobGustavo/Desafio-ForumHub/assets/166851917/f8bb69bc-452d-4604-9804-83d48b3d2392" alt="badge-literalura" width="200"/> <img src="https://github.com/JacobGustavo/Desafio-ForumHub/assets/166851917/8f208ac8-687b-46ee-a2b9-f8d400e05cb5" alt="Badge-Conversor" width="200"/>

## License
 - [License](http://www.apache.org/licenses/LICENSE-2.0)





