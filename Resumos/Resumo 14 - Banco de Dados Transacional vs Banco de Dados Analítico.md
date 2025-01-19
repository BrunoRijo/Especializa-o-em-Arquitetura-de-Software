# Banco de Dados Transacional vs Banco de Dados Analítico
>[!Note]
>Resumo 14 | Especialização em Arquitetura de Software por Bruno Rijo

#### Antes de compreender o que é um banco de dados transacional, é necessário saber o que são transações.

No contexto de BD, transações são grupos de tarefas realizadas no banco de dados, são uma sequência de ações realizadas que não podem ser interrompidas. São usadas para trazer informações, fazer cálculos, etc.. e são específicas para um propósito.

Assim, logicamente sabemos que bancos de dados transacionais, são bancos de dados que executam transações, que resultam em uma resposta e/ou execução de uma determinada tarefa.

As transações devem manter quatro propriedades integradas entre si:
 - Atomicidade: garantia de que a transação será feita por completo.
 - Consistência: Proteção da integridade dos dados.
 - Isolamento: Capacidade de isolar uma transação, garantindo que não haja interferência de/em outras transações.
 - Durabilidade: É a preservação dos dados após as transações terem sido realizadas, garantindo que os resultados sejam salvos e mantidos.

Os sistemas operacionais atuais conseguem executar múltiplas transações, intercalando entre as transações do tipo sequencial e sequencial seriada.

Enquanto os BD relacionais possuem foco nas transações, tarefas que não podem ser fragmentadas, os BD analíticos possuem características que focam na análise dos dados.

Nos BD analíticos é um repositório de dados central que reúne dados integrados vindos de diferentes fontes de dados utilizadas para análises e relatórios. O Objetivo é ser performático enquanto aporta um volume grande de dados.

Dentre as características de bancos de dados analíticos se destacam: 

1️⃣ **Foco em analisar grandes volumes de dados e análise de negócios**

2️⃣ **Otimizado para realizar grandes inserções e selects**

3️⃣ **Performance, realizando consultas em segundos**

#### #SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
