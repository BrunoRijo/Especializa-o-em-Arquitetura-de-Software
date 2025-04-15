# Observer Design Pattern
>[!Note]
>Resumo 41 | Especialização em Arquitetura de Software por Bruno Rijo

Opa, tudo bem?
Falando agora sobre um padrão de projeto comportamental, o Observer!!

Permite que seja definido um mecanismo de assinatura para notificar múltiplos objetos sobre qualquer evento que aconteça com o objeto que estiver sendo observado.

Imagine que voce tem um objeto central e vários módulos do sistema que precisam interagir automaticamente quando algo muda nele? Como um pedido de compra é feito por exemplo, é preciso enviar um email para o cliente, atualizar o estoque, emitir uma NF, notificar o financeiro e etc. Se você implementar isso de forma direta o código do pedido pode virar uma bagunça com várias chamadas muito específicas. O Observer resolveria isso desacoplando os dependentes, ou seja, o pedido não precisa saber quem quer ser notificado, ele apenas emite um evento e as classes observadoras cuidam do resto.

Apesar de ser mais fácil de adicionar ou remover comportamentos novos, pode ser difícil de depurar ou rastrear problemas se houver muitos observadores envolvidos, além de que pode causar problemas de performance em sistemas muito grandes, se não for bem implementado.

A estrutura do Observer envolve os seguintes elementos:
1. Interface Subject (Sujeito observado) - é uma interface que conterá o método que manda eventos de interesse para outros objetos, sendo que esses eventos ocorrerão quando for realizado algum comportamento ou houver alguma mudança de estado.
2. ConcreteSubject - implementa a lógica da interface subject.
3. Interface Observer (Observador) - interface que define o método atualizar() que será chamado pela Interface Subject.
4. Concrete Observe - Todas as classes devem implementar a mesma interface e conterá as ações que serão observadas.
5. Client - que é que monta o esquema.

[Lembrete] Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

No próximo resumo falarei sobre o Memento. :) Até lá.

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
