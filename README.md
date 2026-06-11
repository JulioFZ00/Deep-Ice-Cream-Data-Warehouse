---

# 🍦 Deep-Ice-Cream-Data-Warehouse

--- 

## 📌 Contexto de Negócio

A Deep Ice Cream é uma empresa fictícia do setor varejista de sorvetes.

Com o crescimento da operação, as informações da empresa passaram a ser armazenadas em diversas planilhas Excel independentes, dificultando 
o controle e a consolidação dos dados, além de aumentar o risco de inconsistências e retrabalho na geração de relatórios gerenciais.

Os principais impactos observados foram:

- Dificuldade na consolidação das informações
- Maior risco de inconsistências nos dados
- Retrabalho na geração de relatórios gerenciais
- Limitações para análises de negócio
- Dificuldades de escalabilidade da operação

Diante desse cenário, a diretoria solicitou ao time de dados o desenvolvimento de uma solução capaz de centralizar, organizar
e estruturar as informações da empresa, criando uma base sólida para futuras análises e tomadas de decisão.

---

## 🎯 Objetivo do Projeto

Projetar e implementar um banco de dados relacional para:

- Centralizar os dados da empresa
- Garantir integridade e consistência das informações
- Eliminar redundâncias
- Facilitar consultas analíticas
- Servir como base para futuras análises de negócio

---

## 🏗️ Etapas do Projeto

- Levantamento de requisitos
- Modelagem conceitual
- Modelagem lógica
- Modelagem física
- Implementação em Oracle SQL
- Desenvolvimento de procedures
- Criação de views analíticas
- Carga e validação dos dados

---

## 🗃️ Entidades Modeladas

O banco de dados foi projetado para representar as principais áreas de negócio da empresa, contemplando as seguintes entidades:

- Clientes
- Endereços
- Produtos
- Categorias
- Pedidos
- Itens de Pedido
- Funcionários
- Unidades
- Histórico de Preços

---

## 📐 Visão Geral da Solução

Para atender às necessidades da empresa, foi desenvolvido um banco de dados relacional utilizando Oracle Database.

A solução foi projetada para centralizar as informações de clientes, produtos, pedidos, funcionários e unidades da empresa, garantindo integridade dos dados e suporte para análises futuras.

O desenvolvimento contemplou desde a modelagem conceitual até a implementação física do banco de dados, incluindo regras de negócio, procedures e views analíticas para facilitar a exploração das informações.

A estrutura do projeto foi organizada em três pilares principais:

* Modelagem dos dados
* Implementação do banco de dados
* Dados de origem e carga inicial

---

## 📂 Estrutura do Projeto

```text
Deep-Ice-Cream-Data-Warehouse
│
├── .gitignore
├── README.md
│
├── Modelagem/
│   ├── README.md
│   └── PDF_DIC_RELACIONAL.pdf
│
├── Implementacao/
│   ├── README.md
│   ├── 01_create_schema.sql
│   ├── 02_inserts_base.sql
│   ├── 03_procedures.sql
│   ├── 04_test_procedures.sql
│   ├── 05_drop_schema.sql
│   └── Views_Analiticas/
│
├── Dados_Originais/
│   ├── sales_2023.sql
│   └── sales_2024.sql

```

### Descrição das Pastas

**Modelagem**

Contém a documentação e os diagramas utilizados durante a construção do modelo de dados.

**Implementação**

Contém os scripts SQL responsáveis pela criação do banco de dados, procedures, views e demais objetos implementados.

**Dados_Originais**

Contém os dados utilizados na carga inicial e materiais de apoio relacionados à origem das informações.

```
```
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

## 🔗 Integração com o Projeto de Analytics

O banco de dados desenvolvido neste projeto serviu como base para o projeto Deep-Ice-Cream-Sales-Analytics, onde os dados foram utilizados para análises
exploratórias, geração de indicadores de negócio e construção de modelos de previsão de vendas.

A separação entre os projetos permite representar de forma mais próxima um ambiente corporativo, onde a camada de armazenamento dos dados é desenvolvida
independentemente da camada analítica.







