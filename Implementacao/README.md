---

# ⚙️ Implementação

Esta pasta contém os scripts responsáveis pela implementação física do banco de dados da Deep Ice Cream.

Com base na modelagem desenvolvida na etapa anterior, foram criadas as estruturas necessárias para armazenar e organizar as informações da empresa de forma consistente e escalável.

Além da criação das tabelas e relacionamentos, a implementação contempla regras de negócio, procedimentos automatizados para manipulação dos dados e views analíticas voltadas para consultas e geração de informações estratégicas.

O objetivo desta etapa é transformar o modelo conceitual e lógico em uma solução funcional, capaz de suportar as operações da empresa e servir como base para futuras análises de dados e processos de tomada de decisão.


---

## 🎯 Objetivos da Implementação

- Criar a estrutura física do banco de dados
- Garantir integridade referencial entre as entidades
- Implementar regras de negócio através de procedures
- Realizar a carga inicial dos dados
- Disponibilizar views para análises futuras

---

## 📜 Scripts Disponíveis

A implementação do banco de dados foi dividida em etapas para facilitar a criação, manutenção e validação da estrutura.

**01_create_schema.sql**

Responsável pela criação das tabelas, constraints e relacionamentos do banco de dados.

**02_inserts_base.sql**

Realiza a carga inicial dos dados cadastrais necessários para o funcionamento do sistema.

**03_procedures.sql**

Contém as procedures utilizadas para automatizar inserções e aplicar regras de negócio.

**04_test_procedures.sql**

Executa testes para validação das procedures implementadas.

**05_drop_schema.sql**

Remove os objetos criados no banco de dados, permitindo recriação completa do ambiente quando necessário.

---

## ⚙️ Componentes Implementados

A partir da modelagem definida na etapa anterior, foram implementados os seguintes componentes:

- Tabelas relacionais
- Chaves primárias e estrangeiras
- Constraints de integridade
- Procedures para inserção e manipulação dos dados
- Scripts de carga inicial
- Scripts de validação
- Views analíticas para suporte à tomada de decisão

---

## 🛠️ Tecnologias Utilizadas

### Banco de Dados:

- Oracle Database

### Linguagens:

- SQL
- PL/SQL

### Ferramentas de Desenvolvimento:

- Oracle SQL Developer
- Oracle SQL Developer Data Modeler

### Versionamento:

- Git
- GitHub

---

## 🔄 Business Rules Implemented
- Product prices are versioned using a price history table
- Sales always use the price valid on the order date
- One order may contain multiple items
- Historical sales are not affected by future price changes

## 🛠 Scripts Execution Order
1. `01_create_schema.sql`
2. `02_inserts_base.sql`
3. `03_procedures.sql`
4. `04_test_procedures.sql`
5. `sales_2023.sql`
6. `sales_2024.sql`
7. Views in `views/`

## 📊 Analytical Views
- Revenue per item
- Revenue per order
- Monthly revenue
- Revenue per product per month
- Revenue per customer
- Average ticket
- Product quantity sold

## 🎯 Purpose
This repository was created as a portfolio project to demonstrate SQL and database design skills for data, BI, and backend-oriented roles.
