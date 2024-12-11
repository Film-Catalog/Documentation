📖 Documentação do Sistema de Catálogo de Filmes
1. Introdução e Visão Geral
1.1 Propósito do Sistema
O Catálogo de Filmes é uma aplicação desenvolvida para oferecer aos usuários a possibilidade de explorar, avaliar e comentar filmes, além de manter um registro personalizado de conteúdos. O sistema é projetado para escalabilidade, permitindo futuras extensões para outras mídias, como séries.

1.2 Objetivos
Proporcionar uma interface eficiente e prática para acessar e interagir com o catálogo.
Oferecer dados completos e personalizados sobre filmes.
Garantir arquitetura modular, extensível e fácil de manter.
1.3 Público-Alvo
Cinéfilos que desejam explorar e avaliar filmes.
Desenvolvedores interessados em aprender sobre design e arquitetura de software.
2. Requisitos do Sistema
2.1 Requisitos Funcionais
Cadastro de Entidades:
Inserção de filmes com título, sinopse, gênero, pontuação, data de lançamento, duração, imagens, entre outros.
Registro de usuários (nome e e-mail).
Manipulação de Dados:
Operações CRUD para filmes e usuários.
Interface de Interação:
APIs REST (com possibilidade de extensão para uma interface gráfica).
Relatórios:
Geração de listas de filmes e histórico de avaliações.
2.2 Requisitos Não Funcionais
Padrão de Projeto: Uso de Factory para facilitar a criação de objetos.
Modularidade: Código estruturado em camadas seguindo princípios da orientação a objetos.
Controle de Versão: Histórico de commits organizado no Git.
Escalabilidade: Suporte a grande volume de dados e usuários simultâneos.
Segurança: Autenticação e proteção de dados sensíveis.
3. Arquitetura e Design
3.1 Estrutura Modular
application: Contém o ponto de entrada do programa.
entities: Representa as classes principais, como Movie e User.
factories: Implementa o padrão Factory para criação de objetos.
services: Contém a lógica de negócios.
repositories: Abstrai a interação com o banco de dados.
3.2 Padrão de Projeto Utilizado
Factory Pattern:
Propósito: Centralizar e facilitar a criação de objetos.
Benefícios: Adição de novos tipos de mídia e redução de acoplamento.
4. Implementação
4.1 Tecnologias Utilizadas
Linguagem: Java
Framework: Spring Boot
Banco de Dados: H2 (testes) e PostgreSQL (produção)
Gerenciador de Dependências: Maven
4.2 Classes Principais
Movie: Representa filmes com atributos como título, diretor e gênero.
User: Representa os usuários, armazenando informações de autenticação.
5. Guia de Instalação
Passo 1: Clonar o Repositório
bash
Copiar código
git clone https://github.com/Film-Catalog/BackEndDevelopment
Passo 2: Configurar o Banco de Dados
Adicione no arquivo application.properties:

properties
Copiar código
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.username=sa
spring.datasource.password=
spring.jpa.hibernate.ddl-auto=update
Passo 3: Executar o Projeto
bash
Copiar código
mvn spring-boot:run
6. Testes
Tipos de Testes
Unitários: Verificação de métodos nas classes de serviço.
Integração: Comunicação entre APIs e banco de dados.
Aceitação: Garantia de cumprimento dos requisitos funcionais.
7. Evolução do Projeto
7.1 Adição de Séries
Criar a classe Series estendendo Media.
Atualizar a MediaFactory para suportar objetos do tipo Series.
Expandir os serviços e controllers com endpoints para séries.
7.2 Recursos Futuros
Sistema de recomendação baseado em avaliações.
Integração com APIs externas, como TMDb, para enriquecer os dados de filmes.
8. Manutenção
Revisões contínuas do código com base no feedback dos usuários.
Atualizações regulares da documentação.
Planejamento para novos recursos, como filtros personalizados e análises detalhadas.
🌟 Explore o mundo do cinema com o Catálogo de Filmes!
