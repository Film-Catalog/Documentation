# 🎬 **Catálogo de Filmes**  

🖥️ Componentes e Views mais importantes do Front-End

MovieHomeContainer

📍 Descrição:
Esta é a página principal da aplicação no lado visual. Aqui, todos os filmes recebidos da API do backend são exibidos.

Funcionalidade Principal: Sistema de filtros que permite reconstrução da página em tempo real.
Tecnologias Utilizadas: React para renderização e manipulação de estados.

MovieDescription

📍 Descrição:
Esta view exibe informações detalhadas de um filme individual.

Dados Recebidos:

Informações como título, sinopse, gênero e ano vêm da API do backend em formato JSON.
A imagem também é carregada diretamente do backend.

Funcionalidade:
Permite acesso rápido às informações detalhadas de cada filme.

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
git clone https://github.com/Film-Catalog/BackEndDevelopment
🔧 Passo 2: Configurar o Banco de Dados
Adicione no arquivo application.properties:

properties
Copiar código
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.username=sa
spring.datasource.password=
spring.jpa.hibernate.ddl-auto=update

🚀 Passo 3: Executar o Projeto
bash
Copiar código
mvn spring-boot:run
6️⃣ Testes
🧪 Tipos de Testes
✔️ Testes Unitários: Verificação de métodos nas classes de serviço.
🔗 Testes de Integração: Comunicação correta entre APIs e banco de dados.
✅ Testes de Aceitação: Cumprimento dos requisitos funcionais.
7️⃣ Evolução do Projeto

📌 7.1 Adição de Séries
Criar a classe Series estendendo Media.
Atualizar a MediaFactory para criar objetos do tipo Series.
Expandir serviços e controllers com endpoints para séries.

🌟 7.2 Recursos Futuros
Sistema de recomendação baseado em avaliações.
Integração com APIs externas (ex.: TMDb) para enriquecer dados de filmes.
8️⃣ Manutenção
🔄 Atualização Contínua: Revisão e melhoria do código com base no feedback dos usuários.
📘 Documentação: Atualizações regulares.
🛠️ Suporte a Novos Recursos: Planejamento para inclusão de filtros personalizados e análises detalhadas.
✨ Explore o universo cinematográfico com o Catálogo de Filmes! 🎥
