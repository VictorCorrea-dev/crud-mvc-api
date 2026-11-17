# Comparação entre CRUD com MVC e API

## Introdução

O CRUD representa as operações de criar, consultar, atualizar e excluir informações. O MVC é um padrão que organiza o código em três partes, enquanto uma API permite a comunicação entre diferentes aplicações.

## 1. Quais as diferenças arquiteturais?

O MVC organiza o sistema em três partes: Model, View e Controller. Já a API permite a comunicação entre o front-end e o back-end por meio de requisições HTTP.

**Diferença:** o MVC organiza o código, enquanto a API permite a comunicação entre sistemas.

## 2. Responsabilidades de cada camada?

**No MVC:**
- **Model:** trabalha com os dados e as regras do sistema.
- **View:** apresenta a interface para o usuário.
- **Controller:** recebe as ações do usuário e controla as operações.

**Na API:**
- **Controller:** recebe as requisições.
- **Service:** executa as regras de negócio.
- **Repository:** realiza a comunicação com o banco de dados.
- **Model/Entity:** representa os dados do sistema.

## 3. Relações entre as camadas?

No MVC, a View envia uma ação ao Controller, que utiliza o Model para trabalhar com os dados e retorna o resultado para a View.

Na API, o front-end envia uma requisição ao Controller, que chama o Service e o Repository quando necessário. Depois, a API retorna uma resposta ao front-end.

## 4. Persistência em um banco de dados.

Nos dois modelos, a persistência permite armazenar informações no banco de dados.

No MVC, essa responsabilidade geralmente fica no Model. Já em uma API, normalmente fica na camada Repository, que realiza operações de cadastro, consulta, atualização e exclusão.

## 5. Qual o padrão arquitetural mais utilizado no mercado?

As APIs REST são muito utilizadas atualmente, principalmente por facilitarem a comunicação entre diferentes sistemas. Elas permitem, por exemplo, que um front-end em React se comunique com um back-end desenvolvido em Java com Spring Boot.

## 6. Como testar esta API?

Podemos utilizar o **Postman**, uma ferramenta que permite enviar requisições e verificar as respostas da API.

Os principais métodos são:

- **GET:** consultar informações.
- **POST:** cadastrar informações.
- **PUT:** atualizar informações.
- **DELETE:** excluir informações.

## 7. Como documentar esta API?

Podemos utilizar o **Swagger**, uma ferramenta que apresenta as rotas, os métodos HTTP, os dados necessários e as possíveis respostas da API. Isso facilita o entendimento e a utilização por outros desenvolvedores.

## 8. Como consumir esta API no front-end?

O front-end pode consumir uma API utilizando Fetch API ou Axios, por meio de requisições HTTP. A API processa a solicitação, consulta ou modifica os dados e retorna uma resposta, geralmente em formato JSON, que será apresentada na tela.

---
