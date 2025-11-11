# Fatec Mobile Device Programming - Exemplos de Apps

Este repositório reúne uma coleção de aplicativos desenvolvidos durante a disciplina de Programação para Dispositivos Móveis. Cada projeto demonstra a integração entre um backend **Node.js (API)** e um frontend **Flutter (aplicativo mobile)**, abordando diferentes funcionalidades e casos de uso.

---

## Visão Geral dos Projetos

- **Gerenciador de Tarefas:** Um aplicativo CRUD completo para gerenciar uma lista de tarefas.
- **Catálogo de Produtos:** Demonstra como exibir dados de uma API com suporte a visualização offline.
- **Gerenciador de Contatos:** Focado na sincronização de dados entre um servidor remoto e um banco de dados local (SQLite).
- **Aplicativo de Notícias:** Exibe notícias de uma API e permite salvar artigos como favoritos para leitura offline.

---

## 1. Gerenciador de Tarefas

**Descrição:**
Aplicativo que permite ao usuário criar, visualizar, editar, marcar como concluídas e excluir tarefas. É um exemplo clássico de implementação CRUD (Create, Read, Update, Delete).

### Backend (Node.js)
- **Local:** `task_manager/task-manager-api`
- **Como rodar:**
  1. Navegue até o diretório: `cd task_manager/task-manager-api`
  2. Instale as dependências: `npm install`
  3. Inicie o servidor: `node index.js`
  4. A API estará disponível em: `http://localhost:3000`

### Frontend (Flutter)
- **Local:** `task_manager/task_manager_app`
- **Como rodar:**
  1. Navegue até o diretório: `cd task_manager/task_manager_app`
  2. Instale as dependências: `flutter pub get`
  3. Execute o aplicativo: `flutter run`
  4. Configure o IP da API, caso seja necessário (emulador/dispositivo físico).

---

## 2. Catálogo de Produtos

**Descrição:**
Aplicativo para visualizar uma lista de produtos. Os dados são carregados a partir de uma API e armazenados localmente para permitir a visualização mesmo sem conexão à internet.

### Backend (Node.js)
- **Local:** `product_catalog/product-catalog-api`
- **Como rodar:**
  1. Navegue até o diretório: `cd product_catalog/product-catalog-api`
  2. Instale as dependências: `npm install`
  3. Inicie o servidor: `node index.js`
  4. A API estará disponível em: `http://localhost:3001`

### Frontend (Flutter)
- **Local:** `product_catalog/product_catalog_app`
- **Como rodar:**
  1. Navegue até o diretório: `cd product_catalog/product_catalog_app`
  2. Instale as dependências: `flutter pub get`
  3. Execute o aplicativo: `flutter run`
  4. Configure o IP da API, caso seja necessário (emulador/dispositivo físico).

---

## 3. Gerenciador de Contatos

**Descrição:**
Solução para gerenciar contatos pessoais. O aplicativo sincroniza os dados entre a API e um banco de dados local (SQLite), garantindo que as informações estejam sempre atualizadas e disponíveis offline.

### Backend (Node.js)
- **Local:** `contact_manager/contact-manager-api`
- **Como rodar:**
  1. Navegue até o diretório: `cd contact_manager/contact-manager-api`
  2. Instale as dependências: `npm install`
  3. Inicie o servidor: `node index.js`
  4. A API estará disponível em: `http://localhost:3002`

### Frontend (Flutter)
- **Local:** `contact_manager/contact_manager_app`
- **Como rodar:**
  1. Navegue até o diretório: `cd contact_manager/contact_manager_app`
  2. Instale as dependências: `flutter pub get`
  3. Execute o aplicativo: `flutter run`
  4. Configure o IP da API, caso seja necessário (emulador/dispositivo físico).

---

## 4. Aplicativo de Notícias

**Descrição:**
Aplicativo que exibe uma lista de notícias de uma API. O usuário pode marcar notícias como favoritas, que são salvas em um banco de dados SQLite para acesso rápido e offline.

### Backend (Node.js)
- **Local:** `news-app/news-app-api`
- **Como rodar:**
  1. Navegue até o diretório: `cd news-app/news-app-api`
  2. Instale as dependências: `npm install`
  3. Inicie o servidor: `node index.js`
  4. A API estará disponível em: `http://localhost:3003`

### Frontend (Flutter)
- **Local:** `news-app/news_app`
- **Como rodar:**
  1. Navegue até o diretório: `cd news-app/news_app`
  2. Instale as dependências: `flutter pub get`
  3. Execute o aplicativo: `flutter run`
  4. Configure o IP da API, caso seja necessário (emulador/dispositivo físico).

---

## Observações Gerais
- **Pré-requisitos:** Certifique-se de ter o **Node.js** (para o backend) e o **Flutter** (para o frontend) instalados em sua máquina.
- **Conexão com a API:** Ao executar o aplicativo Flutter em um dispositivo físico, lembre-se de substituir `localhost` pelo endereço IP da máquina onde o servidor Node.js está rodando.
- **Armazenamento Local:** Os dados salvos localmente (via SQLite) são armazenados no próprio dispositivo ou emulador, na área de dados do aplicativo.
