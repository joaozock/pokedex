# 🧩 Pokédex

Aplicação web responsiva desenvolvida para praticar **JavaScript, consumo de APIs e manipulação dinâmica de dados**.

A aplicação utiliza a **PokeAPI** para obter informações dos Pokémon e gerar dinamicamente os cards apresentados na interface.

## ✨ Funcionalidades

* 📱 Interface responsiva
* 🔌 Integração com a **PokeAPI**
* 🔎 Consulta de informações dos Pokémon através de API
* 🃏 Criação dinâmica dos cards
* 🖼️ Exibição da imagem de cada Pokémon
* 🏷️ Exibição do nome, número e tipos
* ⬇️ Carregamento incremental de Pokémon
* ➕ Botão **"Load More"** para carregar novos registros
* ⚡ Processamento de múltiplas requisições utilizando `Promise.all()`

## 🛠️ Tecnologias utilizadas

* HTML5
* CSS3
* JavaScript
* PokeAPI

## 🔌 Consumo da API

A aplicação utiliza a **PokeAPI** para obter os dados dos Pokémon.

O JavaScript realiza as requisições e transforma os dados retornados pela API em objetos utilizados para construir os cards exibidos na página.

O fluxo principal funciona da seguinte maneira:

```text
PokeAPI
   ↓
Requisição HTTP
   ↓
JavaScript
   ↓
Processamento dos dados
   ↓
Criação dos cards
   ↓
Interface
```

## 📊 Carregamento incremental

Para evitar o carregamento de uma grande quantidade de Pokémon de uma só vez, a aplicação utiliza um sistema de carregamento incremental.

Inicialmente são carregados **10 Pokémon**. Ao clicar em **"Load More"**, novos registros são solicitados à API.

```text
Inicial
10 Pokémon
   ↓
Load More
   ↓
+10 Pokémon
   ↓
Load More
   ↓
+10 Pokémon
```

A aplicação utiliza os parâmetros `offset` e `limit` para controlar quais registros devem ser carregados.

## ⚙️ Organização do código

O projeto possui uma separação entre as principais responsabilidades da aplicação:

```text
assets/
└── js/
    ├── main.js
    ├── poke-api.js
    └── pokemon-model.js
```

### `main.js`

Responsável pela interação com a página e pela atualização da interface.

### `poke-api.js`

Responsável pela comunicação com a PokeAPI e obtenção dos dados.

### `pokemon-model.js`

Responsável pela estrutura dos objetos utilizados para representar os Pokémon na aplicação.

## 🎯 Objetivos do projeto

O projeto foi desenvolvido para praticar:

* Consumo de APIs REST
* Requisições HTTP utilizando `fetch()`
* Programação assíncrona com JavaScript
* Utilização de `Promise.all()`
* Manipulação de dados retornados por APIs
* Criação dinâmica de elementos HTML
* Manipulação do DOM
* Organização do código JavaScript
* Desenvolvimento de interfaces responsivas

## 📚 Aprendizados

O desenvolvimento da Pokédex proporcionou prática principalmente com **integração de APIs e manipulação de dados externos**.

Também foi possível trabalhar com programação assíncrona, criação dinâmica de componentes da interface e controle de carregamento dos dados para proporcionar uma experiência mais organizada ao usuário.

## 👨‍💻 Autor

**João Victor Farias Zock**

* GitHub: [@joaozock](https://github.com/joaozock)
* LinkedIn: [linkedin.com/in/joaozock](https://linkedin.com/in/joaozock)
