# Esquema Estrela e Esquema Floco de Neve
>[!Note]
>Resumo 18 | Especialização em Arquitetura de Software por Bruno Rijo

O conceito de esquema estrela, ou Star Schema, propõe uma visão de modelagem de dados que suporta a tomada de decisão orientada a dados, ou seja, uma modelagem dimensional onde se tem a presença de UMA tabela FATO e N tabelas DIMENSÃO, que criam um modelo similar a uma estrela.

![1643281137072](https://github.com/user-attachments/assets/e3a257b9-4ab0-400b-85c7-a5df930ad564)

Dentre as características desse modelo se destacam:
- Uso maior de armazenamento em disco.
- É uma modelagem incremental, onde a novas dimensões podem ser incrementadas no decorrer do tempo.
- É o modelo mais utilizado

Já o esquema Floco de Neve, ou Snowflake Schema, foi criado com a intenção de economizar espaço em disco,e possui as técnicas mais utilizadas para modelagem dimensional.

No modelo estrela, cada dimensão é relacionada apenas com o fato, logo, podem ocorrer redundâncias, diferente do modelo floco de neve onde não há uma regra fixa de normalização, sendo que um ramo do esquema pode ser maior do que o outro, além de que as tabelas podem se relacionar entre si de maneira independente.

Exemplo:
![snowflake-schema-diagram-image](https://github.com/user-attachments/assets/4e6f781a-e61d-4e65-a49e-c7c83f4b2551)

Aqui se encerram os resumos dessa cadeira, a partir do próximo falarei sobre "Arquiteturas e Infraestruturas em Nuvem"!

Até lá. :)

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
