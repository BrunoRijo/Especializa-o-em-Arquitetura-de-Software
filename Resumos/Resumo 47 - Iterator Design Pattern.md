# Iterator Design Pattern
>[!Note]
>Resumo 47 | Especialização em Arquitetura de Software por Bruno Rijo

Opa!! Continuando a saga dos padrões de projeto, vou falar hoje sobre o Iterator.

Esse padrão permite que se possa percorrer elementos de uma coleção sem que seja necessário expor a representação dessas coleções, ou seja, permite que objetos, seja de uma lista, pilha, conjunto ou árvore sejam percorridos um a um sem que o cliente precise saber os detalhes internos da estrutura, como os índices ou nós…

Esse design pattern em específico, dependendo da linguagem já possui implementações em bibliotecas nativas, por exemplo, em Java, C# e até mesmo utilizando Generics nas versões de Delphi menos antigas. No Java temos o List, o Set, Map e Queue, onde todos possuem métodos para iterar automaticamente, assim como no  Delphi, é possível iterar estruturas dos tipos TList e TDictionary.

Mas caso esteja usando uma linguagem sem esse tipo de recurso, seria necessário a seguinte estrutura:
1. Interface Iterator - Para definir os códigos de percorrer os elementos.
2. Concrete Iterator - Que implementa a interface Iterator e mantém o estado da posição atual.
3. Interface Aggregate - Para definir um método para criar o Iterator.
4. Concrete Aggregate - Que implementa a interface e retorna o iterador apropriado.

Bem tranquila a ideia desse padrão né?

No próximo resumo, vou falar sobre o Template Method.

[Lembrete] Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper

Fontes:
- Ferreira, Arthur Gonçalves. F383d - Design Patterns e gerência de configuração: do projeto ao controle de versões / Arthur Gonçalves Ferreira, – São Paulo: Platos Soluções Educacionais S.A., 2021.
- https://docs.oracle.com/en/java/javase/24/
- https://docwiki.embarcadero.com/Libraries/Sydney/en/System.Generics
