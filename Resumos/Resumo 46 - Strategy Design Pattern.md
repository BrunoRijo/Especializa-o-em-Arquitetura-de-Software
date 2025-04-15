# Strategy Design Pattern
>[!Note]
>Resumo 46 | Especialização em Arquitetura de Software por Bruno Rijo

Opa! Continuando a saga dos padrões de projeto comportamentais, vou falar hoje sobre o padrão Strategy.

Esse padrão tem o objetivo de modificar o comportamento de um objeto em tempo de execução. Ele permite que possa ser definida uma família de algoritmos, que pode ser encapsulada em uma classe separada, onde os objetos dentro dessa classe possam ser intercambiáveis. 

Um exemplo, imagine que você está desenvolvendo um e-commerce. O cliente pode pagar de várias formas diferentes, com boleto, Pix, cartão de crédito e etc. Ao invés de adicionar um bloco de if/else no controller, você pode usar o strategy para executar a estratégia mais adequada pro método escolhido, em tempo de execução.

A estrutura básica:

1. Interface Strategy - É comum a todas as estratégias concretas, declara um método que o contexto usa para utilizar uma estratégia.
2. Concrete Strategy -  Cada classe que implementa diferentes variações do algoritmo utilizado pelo contexto.
3. Contexto - É a classe que utiliza o Strategy, ela recebe o comportamento por composição e o utiliza.

No próximo resumo vou falar sobre o iterator.
Te vejo no próximo.

[Lembrete] Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
