# 🗄️ Guia Definitivo de MySQL: Da Modelagem ao SQL Prático

Este repositório é um guia completo e estruturado para o aprendizado de Banco de Dados Relacionais, focado no ecossistema **MySQL**. Ele foi projetado para cobrir desde a fase abstrata de concepção e levantamento de requisitos com o cliente, passando pela modelagem lógica e normalização, até a escrita de scripts SQL avançados e resolução de desafios práticos.

Seja você um estudante consolidando os fundamentos ou um desenvolvedor refinando suas habilidades de design de banco de dados, este espaço serve como um guia de referência rápida e uma trilha de estudos prática.

---

## 🧭 Mapa da Trilha de Aprendizado

O repositório está organizado de forma sequencial para refletir o fluxo de desenvolvimento de um banco de dados no mundo real:

1. **[01-introducao-bd](./01-introducao-bd/)**: O que são Bancos de Dados e a diferença fundamental para os SGBDs.
2. **[02-requisitos-e-modelagem](./02-requisitos-e-modelagem/)**: Como ouvir o cliente, extrair requisitos e convertê-los em regras de negócio.
3. **[03-mer-e-der](./03-mer-e-der/)**: Modelagem Conceitual vs. Modelagem Lógica. Como desenhar diagramas eficientes.
4. **[04-normalizacao](./04-normalizacao/)**: Aplicação prática das Formas Normais (1FN, 2FN e 3FN) para evitar redundâncias e anomalias.
5. **[05-scripts-sql](./05-scripts-sql/)**: Implementação física no MySQL usando comandos DDL, DML e DQL.
6. **[06-exercicios-e-desafios](./06-exercicios-e-desafios/)**: Problemas reais com soluções detalhadas e modelos DER correspondentes.

---

## 📖 Visão Geral dos Módulos

### 🧠 1. Introdução a Banco de Dados e SGBD
Entenda a diferença crucial entre a estrutura de armazenamento e o software que a gerencia:
* **Banco de Dados**: O conjunto de dados estruturados e interrelacionados armazenados logicamente.
* **SGBD (Sistema Gerenciador de Banco de Dados)**: O software responsável por controlar o acesso, segurança, integridade e manipulação desses dados (ex: MySQL, PostgreSQL, SQL Server).

### 👥 2. Engenharia de Requisitos para Dados
A criação de um banco de dados robusto começa fora do código. Aqui abordamos:
* **Interpretação e Escuta Ativa**: Como traduzir as necessidades cotidianas e dores do cliente em requisitos técnicos.
* **Regras de Negócio**: Identificar restrições essenciais (ex: *"Um produto só pode ser vendido se houver estoque"* ou *"Um cliente pode ter múltiplos telefones salvos"*).

### 📐 3. Modelagem Conceitual (MER) vs. Modelagem Lógica (DER)
Entenda como documentar o esqueleto do seu banco em diferentes níveis de abstração:
* **MER (Modelo Entidade-Relacionamento)**: Representação abstrata e semântica de alto nível (focado em Entidades, Atributos e Relacionamentos com os famosos losangos de ligação).
* **DER (Diagrama Entidade-Relacionamento)**: A "planta técnica" lógica do banco de dados, exibindo chaves primárias (PK), chaves estrangeiras (FK), tipos de dados específicos e cardinalidades precisas (usando a notação pé de galinha / *Crow's Foot*).

### 🧹 4. Normalização de Dados (1FN, 2FN, 3FN)
O processo indispensável para garantir a integridade estrutural e a performance do banco de dados:
* **1ª Forma Normal (1FN)**: Eliminação de campos multivalorados e repetitivos. Cada célula deve conter valores atômicos (indivisíveis).
* **2ª Forma Normal (2FN)**: Estar na 1FN e garantir que todos os atributos não-chave dependam totalmente da chave primária (eliminação de dependências parciais).
* **3ª Forma Normal (3FN)**: Estar na 2FN e garantir que atributos não-chave não possuam dependências transitivas entre si.

### 💻 5. Implementação Física e Sintaxe MySQL
Traduzindo o DER para código SQL real. Cobertura abrangente dos principais comandos:
* **DDL (Data Definition Language)**: `CREATE DATABASE`, `CREATE TABLE`, `ALTER TABLE` (com ajustes finos como inserção de `AUTO_INCREMENT` e propriedades `NOT NULL`), `DROP TABLE`.
* **DML (Data Manipulation Language)**: `INSERT INTO`, `UPDATE`, `DELETE`.
* **DQL (Data Query Language)**: `SELECT`, filtros avançados com `WHERE`, ordenações com `ORDER BY`, agrupamentos com `GROUP BY`, e junções de tabelas cruciais com `INNER JOIN`, `LEFT JOIN` e `RIGHT JOIN`.

### 🏆 6. Exercícios Práticos e Desafios
Coloque a mão na massa! Este módulo contém cenários de empresas reais, nos quais você deverá:
1. Ler o estudo de caso do cliente.
2. Criar o desenho conceitual e lógico (DER).
3. Aplicar as formas normais.
4. Escrever o script de criação física do banco.
5. Resolver queries complexas baseadas em perguntas de negócios.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas

* **Banco de Dados**: MySQL Server
* **Interface de Gerenciamento**: MySQL Workbench
* **Ferramenta de Modelagem Visual**: Draw.io (diagrams.net)
* **Controle de Versão**: Git & GitHub

---

## 🤝 Como Contribuir

Fique à vontade para propor melhorias teóricas, novos desafios ou otimização nos scripts SQL!
1. Faça um **Fork** do projeto.
2. Crie uma Branch para sua feature ou correção (`git checkout -b feature/MinhaFeature`).
3. Faça o **Commit** de suas alterações (`git commit -m 'Adicionando desafio X'`).
4. Faça o **Push** para a Branch (`git push origin feature/MinhaFeature`).
5. Abra um **Pull Request**.

---

### ✍️ Autor

Desenvolvido por **Lucas Machado** *Profissional de TI e Docente na área de Tecnologia, focado em ensinar de forma descomplicada e altamente técnica.*

---
