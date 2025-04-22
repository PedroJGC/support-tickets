# 🚀 API de Gerenciamento de Tickets de Suporte

Um sistema de gerenciamento de tickets de suporte técnico, construído com Node.js puro.

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

## 📋 Sobre o Projeto

Esta é uma API RESTful para gerenciamento de tickets de suporte técnico. A aplicação permite criar, listar, atualizar, alterar o status e remover tickets de suporte, proporcionando uma solução eficiente para equipes de suporte técnico.

## 🛠️ Tecnologias Utilizadas

### Core

- **Node.js**: Utilizando apenas módulos nativos sem frameworks externos
- **JavaScript (ESM)**: Código moderno com ECMAScript Modules

### Módulos Nativos

- **node:http**: Para criar o servidor HTTP
- **node:fs/promises**: Para manipulação de arquivos de forma assíncrona
- **node:crypto**: Para geração de IDs únicos (UUID)

### Arquitetura

- **MVC (Model-View-Controller)**: Organização do código em controladores e rotas
- **Middlewares**: Para processamento da requisição e resposta
- **Banco de Dados**: Implementação de um banco de dados em JSON persistido em disco
- **RESTful API**: Endpoints organizados seguindo boas práticas REST

### Ferramentas de Desenvolvimento

- **ESLint**: Para análise estática de código
- **Prettier**: Para formatação consistente do código
- **node --watch**: Para reiniciar automaticamente o servidor durante o desenvolvimento

## 🚀 Funcionalidades

- ✅ **Criar tickets**: Registrar novos chamados de suporte
- 📋 **Listar tickets**: Visualizar todos os tickets com possibilidade de filtros
- 🔄 **Atualizar tickets**: Modificar informações de tickets existentes
- 🔒 **Fechar tickets**: Alterar o status de tickets para fechado
- 🗑️ **Excluir tickets**: Remover tickets do sistema

## 🏗️ Estrutura do Projeto

```
support-tickets/
├── src/
│   ├── controllers/     # Controladores de cada operação
│   ├── database/        # Implementação do banco de dados em JSON
│   ├── middlewares/     # Processamento de requisições
│   ├── routes/          # Definição das rotas da API
│   ├── utils/           # Funções utilitárias
│   └── server.js        # Ponto de entrada da aplicação
├── .eslintrc.json       # Configuração do ESLint
├── .prettierrc          # Configuração do Prettier
└── package.json         # Dependências e scripts
```

## 📝 Como Usar

### Instalação

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/support-tickets.git

# Entre no diretório
cd support-tickets

# Instale as dependências
npm install
```

### Execução

```bash
# Inicie o servidor de desenvolvimento
npm run dev
```

### Endpoints da API

- `POST /tickets` - Criar um novo ticket
- `GET /tickets` - Listar todos os tickets
- `PUT /tickets/:id` - Atualizar um ticket específico
- `PATCH /tickets/:id/close` - Fechar um ticket
- `DELETE /tickets/:id` - Remover um ticket

## 🧠 Destaques Técnicos

- **Roteamento Customizado**: Implementação de sistema de rotas com suporte a parâmetros e query strings
- **Banco de Dados em Memória**: Persistência em arquivo JSON com operações CRUD
- **Parseamento de JSON**: Middleware para processar requisições JSON
- **Arquitetura Limpa**: Separação clara de responsabilidades entre componentes

## 📄 Licença

Este projeto está sob a licença ISC.

---

Desenvolvido por Pedro Carvalho
