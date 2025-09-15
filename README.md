# 📦 Gestor de Estoque — SPA com React + Vite

Bem-vindo ao **Gestor de Estoque**, uma aplicação web single-page (SPA) feita com **Vite + React** e **React Router**. O app permite cadastrar produtos, listar, visualizar detalhes, atualizar e excluir, além de um **dashboard** com métricas úteis.
Todos os dados são **persistidos no `localStorage`** do navegador (sem backend).

---

## 📝 Descrição

O sistema oferece:

* 📊 **Dashboard** com:

  * Total de **itens diferentes** (ex.: 1 mesa + 3 cadeiras = 2 itens).
  * Total de **quantidade em estoque** (ex.: 1 mesa + 3 cadeiras = 4 unidades).
  * **Itens adicionados nos últimos 10 dias** (contagem + lista).
  * **Itens com menos de 10 em estoque** (contagem + lista).
* 🗂️ **Lista de produtos** em tabela com ações: **ver detalhes**, **editar** e **excluir**.
* 🔎 **Detalhes do produto** com todas as propriedades e ações de edição/remoção.
* 🆕 **Criação** de produtos (campos: **nome, quantidade, preço, categoria, descrição**).
* ✏️ **Atualização** de produtos (mesma base do formulário de criação).
* ⚡ Navegação **client-side** usando **React Router** (sem recarregar a página).
* 💾 **Persistência local** via `localStorage`.

---

## 🛠️ Tecnologias

* ![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge\&logo=vite\&logoColor=white) **Vite** – dev server e build
* ![React](https://img.shields.io/badge/React-20232A?style=for-the-badge\&logo=react\&logoColor=61DAFB) **React** – UI
* ![React Router](https://img.shields.io/badge/React%20Router-CA4245?style=for-the-badge\&logo=reactrouter\&logoColor=white) **React Router DOM** – roteamento SPA
* ![JavaScript](https://img.shields.io/badge/JavaScript-000000?style=for-the-badge\&logo=javascript) **JavaScript (ESM)**
* ![ESLint](https://img.shields.io/badge/ESLint-4B32C3?style=for-the-badge\&logo=eslint\&logoColor=white) **ESLint** – qualidade de código

---

## 🗂️ Estrutura de Pastas

```
exercicio-final-gestor-de-estoque/
├─ node_modules/              # Dependências (gerado automaticamente)
├─ public/                    # Assets públicos
├─ src/                       # Código-fonte da aplicação
│  ├─ components/            # Componentes reutilizáveis (Tabela, Botões, Formulários...)
│  ├─ contexts/              # Context API (estado global, storage, etc.)
│  ├─ entities/              # Modelos/contratos dos dados (ex.: Product)
│  ├─ hooks/                 # Hooks customizados (ex.: useLocalStorage, useProducts)
│  ├─ pages/                 # Páginas/rotas (Dashboard, List, Details, Create, Edit)
│  ├─ App.jsx                # Shell da aplicação + layout
│  ├─ index.css              # Estilos globais
│  ├─ main.jsx               # Ponto de entrada (ReactDOM)
│  └─ router.jsx             # Definições de rotas do React Router
├─ .gitignore
├─ eslint.config.js          # Configuração do ESLint
├─ index.html                # HTML base
├─ package.json              # Metadados, scripts e dependências
├─ package-lock.json
├─ README.md                 # Este documento
└─ vite.config.js            # Configuração do Vite
```

---

## 🧭 Rotas Principais

* `/` — **Dashboard**
* `/items` — **Lista** de produtos
* `/items/new` — **Criar** produto
* `/items/:id` — **Detalhes** do produto
* `/items/:id/update` — **Editar** produto

> Todas as rotas são renderizadas via **client-side navigation**.

---

## 🚀 Como Rodar o Projeto

```bash
# 1) Clonar o repositório
git clone https://github.com/RaphaelOkuyama/react-stock.git
cd react-stock

# 2) Executar o app
npm run dev
```

> A aplicação abrirá em: **[http://localhost:5173](http://localhost:5173)**

---

## 📦 Scripts Disponíveis

* `npm run dev` – inicia o Vite (desenvolvimento)
* `npm run build` – gera o build de produção
* `npm run preview` – serve o build localmente
* `npm run lint` – executa o ESLint

---

## 🤝 Contribuições

Sinta-se à vontade para abrir **issues** e enviar **pull requests** com melhorias, correções e novas ideias.

---

## 📄 Licença

Este projeto está licenciado sob a **MIT License**.
Consulte o arquivo [LICENSE](./LICENSE) para o texto completo.

Copyright (c) 2025 Raphael Okuyama
