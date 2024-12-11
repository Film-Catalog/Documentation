# 🎬 **Catálogo de Filmes**  

---

## 📖 **Documentação do Sistema**  

---

## 1️⃣ **Introdução e Visão Geral**

### 🎯 **1.1 Propósito do Sistema**
O **Catálogo de Filmes** é uma aplicação desenvolvida para:
- Permitir aos usuários explorar, avaliar e comentar filmes.  
- Manter um registro personalizado de conteúdos.  
- Ser escalável, possibilitando a inclusão de novas mídias (ex.: séries).  

### 🏆 **1.2 Objetivos**
- 🌟 Proporcionar uma interface eficiente e prática.  
- 📊 Oferecer dados completos e personalizados sobre filmes.  
- 🛠️ Garantir arquitetura modular e fácil de manter.  

### 👥 **1.3 Público-Alvo**
- 🎥 Cinéfilos que desejam explorar e avaliar filmes.  
- 💻 Desenvolvedores interessados em boas práticas de design e arquitetura de software.  

---

## 2️⃣ **Requisitos do Sistema**

### ⚙️ **2.1 Requisitos Funcionais**
- **📋 Cadastro de Entidades:**  
  - Cadastro de filmes com informações detalhadas (título, sinopse, gênero, pontuação, etc.).  
  - Registro de usuários com nome e e-mail.  
- **🔄 Manipulação de Dados:**  
  - Operações CRUD para filmes e usuários.  
- **🌐 Interface de Interação:**  
  - APIs REST para comunicação (opcionalmente adaptável a interfaces gráficas).  
- **📑 Relatórios:**  
  - Geração de listas de filmes e histórico de avaliações.  

### 🔒 **2.2 Requisitos Não Funcionais**
- **🏗️ Padrão de Projeto:** Implementação do padrão **Factory** para criar objetos.  
- **📂 Modularidade:** Código estruturado seguindo princípios de orientação a objetos.  
- **📜 Controle de Versão:** Histórico organizado de commits no Git.  
- **📈 Escalabilidade:** Suporte a grande volume de dados e usuários simultâneos.  
- **🔐 Segurança:** Autenticação e proteção de dados sensíveis.  

---

## 3️⃣ **Arquitetura e Design**

### 🧩 **3.1 Estrutura Modular**
Organização em pacotes com responsabilidades claras:  
- **📂 application:** Ponto de entrada do programa.  
- **📂 entities:** Classes principais como `Movie` e `User`.  
- **📂 factories:** Implementação do padrão Factory para criação de objetos.  
- **📂 services:** Lógica de negócios.  
- **📂 repositories:** Abstração da interação com o banco de dados.  

### 🛠️ **3.2 Padrão de Projeto Utilizado**
- **Factory Pattern:**  
  - **Propósito:** Centralizar e facilitar a criação de objetos.  
  - **Benefícios:**  
    - Adição de novos tipos de mídia, como séries.  
    - Redução de acoplamento entre lógica de negócios e criação de objetos.  

---

## 4️⃣ **Implementação**

### 💻 **4.1 Tecnologias Utilizadas**
- **🖥️ Linguagem:** Java  
- **📦 Framework:** Spring Boot  
- **💾 Banco de Dados:** H2 (testes) e PostgreSQL (produção)  
- **⚙️ Gerenciador de Dependências:** Maven  

### 🧑‍💻 **4.2 Classes Principais**
- **🎥 Movie:** Representa filmes com atributos como título, diretor e gênero.  
- **👤 User:** Representa os usuários do sistema com informações de autenticação.  

---

## 5️⃣ **Guia de Instalação**

### 📝 **Passo 1: Clonar o Repositório**
```bash
git clone https://github.com/Film-Catalog/BackEndDevelopment
