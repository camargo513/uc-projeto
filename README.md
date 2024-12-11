# API de carros - webAPI

Está é uma API RESTful desenvolvida paraq gerenciamento de informações de carros, utilizando **NODE.js** e **Express**. A API permite criar, ler, autualizar e excluuir carros, com validação dos dados utilizando a biblioteca **Joi**.

Este é um projeto inicial de CRUD ( Create, Read, Update), que será expandido no futuro. Esta é apena inicial.

## fucionalidades

-**GET /**: retorna a lista completa de carros.
-**GET /:sigla**: Retorna as informações de um carro especifico, identifiqye pela sigla
-**POST /**: adiciona um novo carro á lista.
-**put /:sigla**: atualiza as informaç~es de um carro especifico, identificado pela sigla.
-**DELETE /:sigla**: remove um carro especifico pela sigla.

## Estrutura do projeto
-**app.js**: Arquivo principal que configura o servidor Wxpress e as rotas da API
-**tabelacarros.js**: contém as validações Joi para os dados dos carros.

## endpoints

### 1. **GET /**

retorna a lista completa de carros disponiveis.

### EXemplo de resposta:

```json

[
    {
       "nome": "ferrari",
       "sigla": "FER",
       "velocidadeMaxima": 340,
       "potencia": 800,
       "consumo": 5.5,
       "aceleracao": 2.9,
       "preco": 3000000
    },
]
```