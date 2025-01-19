# Fundamentos de Modelagem de dados para um Data Warehouse
>[!Note]
Resumo 17 | Especialização em Arquitetura de Software por Bruno Rijo

Há dois modelos de modelagem de dados dimensionais para um DW, são eles o modelo Estrela e o Floco de Neve. 

Mas antes de entender como aplicar esses modelos, é necessário entender como os dados devem ser preparados para que possam ser utilizados neles.

Os dois principais elementos, que são a tabela “Fato” e a tabela “Dimensão”.

A tabela Fato, corresponde ao que queremos representar de fato, enquanto a tabela dimensão diz respeito a manipulação da forma como o fato será entregue.

Exemplo: Suponha que você precise de um relatório de vendas de um determinado período, será necessário uma tabela de dimensão que traga uma relação dos dados com o tempo.. se fosse um relatório de vendas por região, seria necessário uma tabela dimensão relacionada com o local especificado, para que possa então manipular dos dados na tabela Fato e entregar o relatório naquela perspectiva. Nesse caso, o fato seria “Vendas” e as dimensões a forma que os dados serão montados para que o fato seja especificado. 

A tabela fato armazena as informações de métricas e chaves estrangeiras, e se complementam com as tabelas dimensão

Uma dimensão, ou qualificador, descreve o fato e contém características do evento, as tabelas dimensão atuam qualificando, classificando e/ou descrevendo os dados, que estão nas tabelas “fato”. Uma dimensão é definida a partir daquilo que o usuário deseja mensurar.

Cada tabela dimensão armazena informações de Surrogate Key (Chave artificial autoincremental), Primary Key, e os atributos.

Por enquanto guarda esses dois conceitos, que no próximo resumo trago a aplicação deles nos modelos de dados.

Até lá. :)

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github.
Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
