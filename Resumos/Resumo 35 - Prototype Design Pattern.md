# Prototype Design Pattern
>[!Note]
>Resumo 35 | Especialização em Arquitetura de Software por Bruno Rijo

Seguindo ainda nos padrões do tipo criancionais, hoje vou falar um pouco sobre o Prototype.

O Prototype é um padrão que tem como objetivo criar novos objetos através da clonagem de um objeto já existente, que é o protótipo. Em vez de instanciar diretamente uma classe, ele utiliza uma cópia de uma instância pré-existente como modelo.

Ele é útil quando a criação direta de um objeto é complexa ou consome muitos recursos, tipo, cálculos complexos, configurações ou acesso a algum recurso externo.

Pra compreender melhor, vou fazer uma analogia aqui, imagine que no sistema em que você atua exista geração de relatórios, onde cada relatório pode conter gráficos, tabelas e várias configurações complexas. Criar relatórios do zero toda vez pode ser demorado. Nesse caso, você poderia criar um protótipo para um relatório genérico com todas as configurações básicas, e quando fosse necessário criar um novo relatório bastaria clonar o protótipo e ajustar apenas algumas informações específicas como os dados enviados para a montagem do gráfico ou tabela.

Uma boa vantagem do uso desse padrão é que se evita a criação repetitiva de novos objetos, já que se usa um modelo genérico pronto, e também o desempenho do código, uma vez que é mais rápido clonar um objeto existente e mudar alguns detalhes do que criar do zero.

Na estrutura básica desse padrão temos as seguintes classes.
1. Interface prototype que possui um método de Clone.
2. Classe concreta que implementa o método clone da interface Prototype.
3. Uma classe cliente que solicita a clonagem dos objetos chamando o método clone.

[Lembrete] Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

No próximo resumo vou falar sobre o Adapter, até o próximo. :)

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
