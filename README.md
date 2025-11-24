# 💻 WEB 2 - PROJETO FINAL

## ✨ Descrição do Projeto

Este projeto consiste em um sistema completo, desenvolvido como requisito final para a disciplina de **WEB 2**. A aplicação é construída com uma arquitetura moderna, englobando as três camadas principais de desenvolvimento: **frontend**, **backend** e **banco de dados**.

O **Sistema de Gerenciamento Acadêmico (SGA)** é uma aplicação full-stack desenvolvida para gerenciar entidades de uma instituição de ensino (Cursos, Alunos e Professores). O objetivo principal é implementar um sistema CRUD (Create, Read, Update, Delete) completo, utilizando arquitetura MVC e garantindo a integridade de dados através de relacionamentos em banco de dados relacional (chaves estrangeiras) e segurança por meio de autenticação de usuários.

Em um contexto real, sistemas como o SGA desempenham papel crucial no gerenciamento eficiente de instituições educacionais, otimizando processos, reduzindo erros operacionais e facilitando o acesso seguro a informações relevantes. Portanto, além de cumprir os requisitos acadêmicos, este projeto também destaca a relevância prática de soluções web bem estruturadas no ambiente educacional moderno.

* **Frontend (Interface do Usuário):** Responsável pela interação visual e experiência do usuário (UX/UI).
* **Backend (Servidor/API):** Gerencia a lógica de negócio, a autenticação, a autorização e a comunicação com o banco de dados.
* **Banco de Dados:** Armazena e gerencia os dados persistentes da aplicação.

---

## 👥 Integrantes do Grupo

Este projeto foi desenvolvido em conjunto pelos seguintes membros:

* Carlos Henrique Moreira Gonçalves
* Gustavo Alves dos Santos
* Guilherme Augusto Frazão Ribeiro
* Henrique Carvalho de Andrade
* Kendy de Oliveira Outi

| Papel Principal | Nome | Contribuição |
| :--- | :--- | :--- |
| **Full-Stack** | Henrique Carvalho | Arquitetura geral, Configuração de ambiente e Backend |
| **Frontend** | Carlos Henrique; Gustavo Alves | Desenvolvimento da interface do usuário e Componentes React |
| **Backend** | Guilherme Augusto; Henrique Carvalho | Implementação das APIs RESTful e Lógica de Negócio |
| **Database** | Kendy Outi | Modelagem do banco de dados e Configuração de ambiente |
| **Documentação** | Kendy Outi | Elaboração do README |

---

## ⚙️ Instruções de Instalação e Execução

### 1. Pré-requisitos

Certifique-se de que os seguintes softwares estão instalados no seu ambiente local antes de prosseguir:

* Node.js 
* npm 
* MySQL 
* Git 
* Um editor de código (como VS Code, Sublime, etc) e terminal de linha de comando.

### 2. Clonagem do Repositório

Abra o terminal e execute os seguintes comandos para obter o código-fonte no seu computador:

```bash
git clone https://github.com/guifrazao/AvaliacaoWEB2.git
cd AvaliacaoWEB2
```

### 3. Configuração do Banco de Dados

1. Crie um banco de dados (por exemplo: `sga_db`).
2. Configure as credenciais de acesso (usuário, senha, host, porta) conforme o seu sistema de banco de dados.
3. Localize o arquivo de configuração do backend (por exemplo `config/db.js`, `.env`, ou similar) e ajuste para apontar para o banco recém-criado.
4. Se houver scripts de migração ou seed (população inicial), execute-os para preparar as tabelas e relacionamentos (chaves estrangeiras, etc).

   ```bash
   # Exemplo genérico, adapte conforme o seu projeto:
   npm run migrate
   npm run seed
   ```

### 4. Instalação e Execução do Backend

1. Navegue até o diretório do backend (por exemplo `sga-backend`)

   ```bash
   cd sga-backend
   ```
2. Instale as dependências:

   ```bash
   npm install
   ```
3. Configure quaisquer variáveis de ambiente necessárias (por exemplo em `.env`):

   ```
   PORT=4000
   DB_HOST=localhost
   DB_PORT=5432
   DB_USER=usuario
   DB_PASSWORD=senha
   DB_NAME=sga_db
   JWT_SECRET=algumSegredo
   ```
4. Inicie o servidor backend:

   ```bash
   npm start
   ```

   O servidor ficará disponível em `http://localhost:4000` (ou outra porta conforme a configuração).

### 5. Instalação e Execução do Frontend

1. Em outro terminal, navegue até o diretório do frontend (por exemplo `sga-frontend`):

   ```bash
   cd ../sga-frontend
   ```
2. Instale as dependências:

   ```bash
   npm install
   ```
3. Ajuste o endpoint da API se for necessário (geralmente em um arquivo como `src/config.js` ou `.env`):

   ```env
   REACT_APP_API_URL=http://localhost:4000/api
   ```
4. Inicie a aplicação frontend em modo de desenvolvimento:

   ```bash
   npm start
   ```

   A interface abrirá no navegador em `http://localhost:3000` (ou outra porta configurada).
5. Acesse e teste o fluxo da aplicação: cadastro, login, CRUD de Cursos/Alunos/Professores, etc.



