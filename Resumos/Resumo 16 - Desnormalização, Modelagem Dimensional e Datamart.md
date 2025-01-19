# Desnormalização, Modelagem Dimensional e o Datamart 
>[!Note]
>Resumo 16 | Especialização em Arquitetura de Software por Bruno Rijo

**Datamart**

A gente já sabe que um data warehouse é um conjunto de elementos e uma preparação de dados para que o usuário consiga realizar consultas performáticas…

Um datamart pode ser definido como uma parte do data warehouse, enquanto o DW é um grande repositório de dados de toda a empresa, o datamart contém um subconjunto desses dados, focado em uma área funcional.

**Desnormalização de dados, o que é Para? que Serve?**

Em um banco de dados transacional, os dados são normalizados, ou seja, as informações são divididas em várias tabelas menores, seguindo um conjunto de regras como atomicidade, eliminação de redundâncias, etc. A desnormalização é o processo de combinar ou simplificar tabelas normalizadas de um banco de dados, com o objetivo de melhorar o desempenho de consultas e geração de relatórios. Assim os dados são armazenados na DW desnormalizados com esse objetivo, já que se lida com uma quantidade MASSIVA de dados.

Desnormalizar os dados além de melhorar a performance, tornando as velocidade das consultas significativamente mais rápidas, também torna as consultas mais simples, com menos necessidade de operações de joins entre as tabelas. 

Em contraponto, lidar com dados desnormalizados pode ocasionar maior redundância,uma vez que desnormalizar cria muitas duplicidades de dados, aumentando o espaço de armazenamento utilizado. Além do risco de inconsistências, já que uma vez que os dados podem ser armazenados em vários locais diferentes, pode ser difícil manter todos atualizados de forma consistente.

**Modelagem dimensional**

Tem objetivo de organizar e permitir melhor desempenho e organização dos dados, que muitas vezes, são provindos de várias fontes, basicamente a modelagem dimensional seria a especificação de uma arquitetura para o DW.

A arquitetura de um DW é dividida em três partes:
- Data source, são as fontes de dados necessárias.
- Staging area, é onde acontece o processo de limpeza e desnormalização dos dados e o carregamentos dos mesmos, para que então possa ser gerado os data mart e o DW.
- Data mart e Data warehouse

Até o próximo :)

#### #SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
