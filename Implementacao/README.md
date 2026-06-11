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

### 01_create_schema.sql

Responsável pela criação das tabelas, constraints e relacionamentos do banco de dados.

### 02_inserts_base.sql

Realiza a carga inicial dos dados cadastrais necessários para o funcionamento do sistema.

### 03_procedures.sql

Contém as procedures utilizadas para automatizar inserções e aplicar regras de negócio.

### 04_test_procedures.sql

Executa testes para validação das procedures implementadas.

### 05_drop_schema.sql

Remove os objetos criados no banco de dados, permitindo a recriação completa do ambiente quando necessário.

### sales_2023.sql

Contém a carga dos dados históricos de vendas referentes ao ano de 2023.

### sales_2024.sql

Contém a carga dos dados históricos de vendas referentes ao ano de 2024.

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

## 🔄 Regras de Negócio Implementadas

Durante a implementação do banco de dados, foram aplicadas regras de negócio para garantir a consistência das informações e preservar o histórico das
operações realizadas.

As principais regras implementadas foram:

* Os preços dos produtos são controlados por meio de uma tabela de histórico de preços.
* Cada venda utiliza o preço vigente na data em que o pedido foi realizado.
* Um pedido pode conter múltiplos itens.
* Alterações futuras de preço não afetam vendas já registradas.
* Os relacionamentos entre as entidades são controlados por constraints de integridade referencial.

---

📊 Views Analíticas

Para facilitar consultas e análises de negócio, foram desenvolvidas views específicas voltadas para indicadores operacionais e comerciais.

As principais views disponibilizadas são:

- Faturamento por Item
- Faturamento por Pedido
- Faturamento Mensal
- Faturamento por Produto e Mês
- Faturamento por Cliente
- Ticket Médio
- Quantidade Vendida por Produto

Essas views servem como camada de apoio para análises futuras e para o projeto Deep-Ice-Cream-Sales-Analytics.

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

🔗 Próxima Etapa

Após a implementação do banco de dados e carga dos dados históricos, as informações passaram a estar disponíveis para análises exploratórias e construção
de modelos preditivos.

Esses dados foram utilizados no projeto Deep-Ice-Cream-Sales-Analytics, responsável pela geração de indicadores de negócio, análises de desempenho e
previsões de vendas.

