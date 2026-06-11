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

## 🏗️ Escopo do Projeto

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

## 📐 Modelagem

Após o levantamento dos requisitos de negócio, foi realizada a modelagem do banco de dados com o objetivo de representar os principais processos da
empresa, garantindo integridade, escalabilidade e suporte para futuras análises.

### Entidades Geográficas

Para evitar redundâncias e garantir consistência dos dados de localização, foi criada uma estrutura hierárquica composta por:

- Estado
- Cidade
- Bairro
- Logradouro

Essa abordagem permite reutilização de informações geográficas e facilita futuras expansões do sistema.


<img width="1024" height="803" alt="Captura de tela 2026-06-11 081439" src="https://github.com/user-attachments/assets/731fe434-576b-4dbe-ab13-6f80b620f0bb" />



