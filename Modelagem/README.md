---

# 📐 Documentação da Modelagem

---

Após o levantamento dos requisitos de negócio, foi realizada a modelagem do banco de dados com o objetivo de representar os principais processos da
empresa, garantindo integridade, escalabilidade e suporte para futuras análises.

## Entidades Geográficas

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
  <img width="900" height="550" alt="Entidades_Geograficas" src="https://github.com/user-attachments/assets/83d1ab22-459a-4f90-934a-5e57c9a64948" />
</p>

---
