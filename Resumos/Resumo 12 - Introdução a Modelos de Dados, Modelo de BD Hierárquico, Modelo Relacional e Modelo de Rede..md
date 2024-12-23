# Introdução a Modelos de Dados, Modelo de BD Hierárquico, Modelo Relacional e Modelo de Rede.
>[!Note]
>Resumo 12 | Especialização em Arquitetura de Software por Bruno Rijo

As informações dos usuários são armazenadas em um banco de dados. É importante saber que esse banco de dados segue um modelo, que é uma estrutura lógica que inclui relacionamentos, tipos de dados e regras que determinam como essas informações podem ser armazenadas ou acessadas.

São diversos os modelos de banco de dados existentes, e cada modelo é tratado de forma individual e é projetado com base em regras e conceitos que são definidos pelos projetistas na fase de modelagem do sistema, assim como para cada modelo desse há um diagrama de banco de dados associado. Os diagramas de banco de dados são uma representação visual de sua estrutura, suas dependências, e de seus relacionamentos. Nesse sentido, o uso de um SGBD (Software de Gerenciamento de Banco de Dados) é muito bem vindo.

Vou falar um pouco dos modelos mais comuns, dentre os vários existentes, começando pelo modelo de banco de dados hierárquico. 

1. O modelo hierárquico organiza os dados em uma estrutura em forma de árvore, onde cada registro possui um único pai ou raiz. Os registros são classificados por meio de especificação de suas entidades e de seus relacionamentos.
  Atualmente esse modelo está em desuso, por conta de ineficiências operacionais, podendo ser visto no mercado somente em sistemas egados…
![db2_novo_banco_dados_hierarquico](https://github.com/user-attachments/assets/d9329c0e-9be0-4c4d-bf4c-5dbdf2305429)

2. Já o modelo relacional é o mais utilizado atualmente, ele classifica os dados em tabelas, também chamadas de relações, compostas por linhas e colunas, onde cada coluna lista um atributo da entidade como id, preço, nome do produto, data de vencimento etc.. nesse modelo, cada linha é chamada de tupla e contém dados sobre o atributo representado na coluna em que se encontra.  Os relacionamentos são feitos através de chaves estrangeiras e podem ser feitos de diversas maneiras como já abordei em outros resumos (1:1, 1:N: N:1, N:N).
Podem ainda ser implementadas regras de normalização com objetivo de aprimorar o desempenho e evitar redundâncias. Os bancos de dados relacionais geralmente são gravados em SQL (Structured Query Language).
![m-jm1](https://github.com/user-attachments/assets/08d72b60-fab1-4f7b-a38e-ce3b3be66d81)

3. O Modelo de Rede, permite relações complexas, é baseado no modelo hierárquico, permitindo relacionamentos de N:N, exemplo: Vários empregados podem fazer parte de vários departamentos, ou seja, serão necessários vários registros pai.
   ![images](https://github.com/user-attachments/assets/eaa3b0f5-2cce-42dd-ac02-0f13a1eb58f8)


