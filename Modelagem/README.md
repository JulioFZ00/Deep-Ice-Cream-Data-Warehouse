---

# 📐 Documentação da Modelagem

---

Após o levantamento dos requisitos de negócio, foi realizada a modelagem do banco de dados com o objetivo de representar os principais processos da
empresa, garantindo integridade, escalabilidade e suporte para futuras análises.

## 🌎 Entidades Geográficas

Para evitar redundâncias e garantir consistência dos dados de localização, foi criada uma estrutura hierárquica composta por:

- Estado
- Cidade
- Bairro
- Logradouro

Essa abordagem permite reutilização de informações geográficas e facilita futuras expansões do sistema.

lém disso, foram criadas estruturas específicas de endereço para clientes, funcionários e unidades da empresa (DIC_END_CLI, DIC_END_FUNCI e DIC_END_UNI).
Essa separação permite manter a integridade referencial de cada entidade, tornando o modelo mais organizado e facilitando a aplicação de regras de negócio
específicas para cada tipo de cadastro.

Como resultado, a modelagem garante maior consistência dos dados e evita a repetição de informações de localização ao longo do banco de dados.

<p align="center">
  <img width="900" height="600" alt="Entidades_Geograficas" src="https://github.com/user-attachments/assets/83d1ab22-459a-4f90-934a-5e57c9a64948" />
</p>

---

## 👥 Entidades com Endereço

Para garantir flexibilidade e reutilização da estrutura geográfica, foram criadas tabelas específicas de endereço para clientes, funcionários e unidades da
empresa.

Clientes:
- Dados cadastrais dos clientes.
- Endereços armazenados em DIC_END_CLI.
  
Funcionários:
- Dados dos colaboradores.
- Endereços armazenados em DIC_END_FUNCI.
  
Unidades:
- Representam lojas e centros de distribuição.
- Endereços armazenados em DIC_END_UNI.

<p align="center">
  <img width="900" height="600" alt="Entidades_Pessoas" src="https://github.com/user-attachments/assets/7cb71942-03dc-4c16-aade-7e3592a44c9e" />
</p>

---

## 🍦 Produtos, Categorias e Processo de Vendas

A estrutura comercial do banco de dados foi projetada para representar o catálogo de produtos da empresa, suas categorias, o histórico de preços praticados
e todo o processo de vendas.

Os produtos são organizados por meio da entidade Categoria, que permite agrupar itens com características semelhantes, facilitando consultas analíticas e
futuras expansões do portfólio.

Além disso, foi criada uma tabela específica de Histórico de Preços, responsável por armazenar as alterações de custo e preço de venda dos produtos ao
longo do tempo. Essa abordagem garante que mudanças futuras de preço não impactem registros históricos de vendas, preservando a consistência das análises
realizadas.

O processo de vendas foi modelado através das entidades:

- Pedido
- Item Pedido
- Produto
- Categoria
- Histórico de Preços

<p align="center">
  <img width="900" height="475" alt="Entidades_produtoo" src="https://github.com/user-attachments/assets/f7f42c8d-c087-4717-b774-cfcb4aca015e" />
</p>

A entidade Pedido representa a transação realizada pelo cliente, enquanto Item Pedido permite que um mesmo pedido contenha múltiplos produtos. Essa
estrutura reproduz o comportamento encontrado em sistemas reais de vendas e garante maior flexibilidade para consultas e análises futuras.

Como resultado, a modelagem permite acompanhar o histórico comercial da empresa, analisar o desempenho dos produtos e preservar a integridade das
informações financeiras ao longo do tempo.

---

## 🔗 Relação com a Implementação

A partir da modelagem apresentada, foram desenvolvidos os scripts SQL responsáveis pela criação das tabelas, definição de constraints, carga inicial dos dados e construção das views analíticas.

Os scripts estão disponíveis na pasta [`Implementacao`](../Implementacao).

---

