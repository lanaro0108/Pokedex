# 📘 Pokédex em Node.js

Este projeto é uma **Pokédex simples no terminal**, desenvolvida em **JavaScript (Node.js)**, que consome a API pública **PokeAPI** para buscar informações sobre um Pokémon digitado pelo usuário.

---

## 🚀 Funcionalidades

* 🔍 Buscar Pokémon pelo **nome**
* 📊 Exibir:

  * Nome
  * Tipos
  * Habilidades
  * Movimentos (limitados a 10)
  * Cadeia de evoluções
* 🔗 Integração com a **PokeAPI**
* ⚡ Uso de `async/await` para requisições assíncronas

---

## 🛠️ Tecnologias utilizadas

* Node.js
* JavaScript
* API REST (PokeAPI)
* Biblioteca `prompt-sync`

---

## 📦 Instalação

1. Clone o repositório ou copie o código
2. Instale as dependências:

```bash
npm install prompt-sync
```

> ⚠️ Se estiver usando Node abaixo da versão 18, instale também o `node-fetch`:

```bash
npm install node-fetch
```

---

## ▶️ Como executar

No terminal, rode:

```bash
node nome_do_arquivo.js
```

Depois, digite o nome do Pokémon quando solicitado:

```
Digite o nome do Pokémon: pikachu
```

---

## 📌 Exemplo de saída

```
================ POKEDEX ================

Nome: pikachu

Tipos:
- electric

Habilidades:
- static
- lightning-rod

Movimentos (golpes):
- mega-punch
- thunder-punch
...

Evoluções:
- pichu
- pikachu
- raichu

=========================================
```

---

## 🧠 Como funciona o código

### 🔹 `buscarEvolucoes(url)`

* Recebe a URL da cadeia evolutiva
* Percorre os estágios do Pokémon
* Retorna um array com todas as evoluções

### 🔹 `pokedex()`

* Solicita o nome do Pokémon
* Faz 3 requisições:

  1. Dados do Pokémon
  2. Dados da espécie
  3. Cadeia de evolução
* Organiza e exibe os dados no console

---

## ❌ Tratamento de erros

Caso o Pokémon não exista ou ocorra erro na API:

```
❌ Pokémon não encontrado ou erro na API
```

---

## 📚 API utilizada

* https://pokeapi.co/

---

## 💡 Possíveis melhorias

* Buscar por **ID**
* Adicionar imagens do Pokémon
* Interface gráfica (GUI)
* Listar todos os movimentos
* Mostrar stats (HP, ataque, defesa, etc.)

---

## 👨‍💻 Autor

Desenvolvido por Pedro Lanaro para fins de estudo e prática com APIs e Node.js.
