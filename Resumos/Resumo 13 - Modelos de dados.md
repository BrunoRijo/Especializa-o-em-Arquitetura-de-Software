# Modelos de dados

>[!Note]
>Resumo 13 | Especialização em Arquitetura de Software por Bruno Rijo

### O modelo de banco de dados orientado a objetos
O modelo de banco de dados orientado a objetos é o modelo pós-relacional mais conhecido, ele incorpora tabelas mas não se limita a elas, esses modelos também são conhecidos como modelos de BD híbridos, pois podem conter arquivos de imagem, áudio, vídeo ou hipertexto.

### Modelo de relacionamento entre as entidades (MER)
Esse modelo captura as relações entre entidades do mundo real muito parecidas com o modelo de rede, mas não está ligado diretamente à estrutura física do BD e sim ao lado conceitual, auxiliando nas visões dos relacionamentos entre as tabelas e a construção de novas visões.

Os dados armazenados em tabelas são o que conhecemos por ENTIDADES e cada uma possui certos atributos que quando unidos formam o DOMÍNIO. Exemplo: A entidade Pessoa possui os atributos nome e CPF, já a entidade Endereço possui a rua, numero e CEP. A cardinalidade também deve ser mapeada, por exemplo, uma pessoa pode possuir mais de um endereço para contato.


Cada entidade pode possuir chave primária que indica a unicidade do conjunto e chave estrangeira para criar relacionamentos entre as tabelas.

![image](https://github.com/user-attachments/assets/e537e392-db10-47c3-85df-b29df30c39c4)

### Modelo estrela
As estruturas que armazenam os dados conhecidos como “dimensões” e os “fatos” são componentes complementares e dependentes entre si, as dimensões fornecem o contexto e as características dos dados, enquanto os “Fatos” são tabelas que guardam informações de quantidades como eventos ou transações. Em um modelo estrela é obrigatória a existência de ambos. Esses elementos são fundamentais para a compreensão e análise das informações. 

Exemplo:

![image](https://github.com/user-attachments/assets/27844d95-1dd4-492d-a336-fd57148c4081)

### Modelo multidimensional
O modelo multidimensional é utilizado principalmente em sistemas de data warehousing e análise de dados. Ele organiza os dados em um formato de "cubo", onde as dimensões representam diferentes perspectivas, como tempo, localização ou produto, e os dados em si, chamados de "fatos", são os valores numéricos, como vendas ou lucros. Esse modelo facilita a análise de grandes volumes de dados de forma rápida e eficiente, permitindo consultas OLAP (Online Analytical Processing) para identificar padrões e tendências ao longo de várias dimensões simultaneamente.

### Modelo de BD NoSQL
Um banco de dados NoSQL, ou Não relacional, é um tipo de banco de dados projetado para lidar com grandes volumes de dados não estruturados ou semiestruturados, oferecendo escalabilidades e uma performance bem melhor em comparação aos modelos relacionais. São ideais para aplicações que requerem grandes quantidades de dados distribuídos.
