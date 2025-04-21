# Chain Of Responsability Design Pattern
>[!Note]
>Resumo 40 | Especialização em Arquitetura de Software por Bruno Rijo

Opa! Tudo bem? 

Bora falar sobre o Chain of Responsability ? Acredito que esse é um dos padrões que tem a ideia mais simples.

Ele permite realizar requisições através de uma corrente de objetos, onde cada objeto decide se vai processar o pedido ou passar adiante para o próximo objeto na corrente. Ele resolve cenários onde você não queria acoplar diretamente o problema ao destinatário final, e precisa que vários outros objetos possam tentar lidar com a requisição, mas sem saber exatamente qual irá lidar com ela.

Um exemplo bem simples, é uma classe de validação de dados antes de realizar um cadastro, você precisa verificar se o email é válido, se a senha é forte, se o CPF é válido e etc .. e você pode sim colocar tudo isso em um único método, mas isso faria que com esse método virasse o que chamam de “God Method” bagunçado, difícil de manter e testar dependendo da aplicação.

A vantagem é a flexibilidade e evitar código procedural enorme com inúmeros if’s, mas ao mesmo tempo pode ser difícil de debugar se a cadeia for muito longa ou dinâmica.

A estrutura básica é composta por:
1. Handler (Objeto Manipulador) - declara o que a interface tem em comum a todos os demais manipuladores concretos, geralmente possui somente uma classe para lidar com pedidos.
2. Classe Cliente - pode compor correntes, apenas uma vez ou de maneira dinâmica.
3. ConcreteHandler (Manipuladores concretos) - que contém código real para processar pedidos, cada manipulador decide se vai processar ou passar para o próximo da corrente.

No próximo resumo, falarei sobre o Padrão Observer.
até lá :) 

[Lembrete] Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

Fonte:
- Ferreira, Arthur Gonçalves. F383d - Design Patterns e gerência de configuração: do projeto ao controle de versões / Arthur Gonçalves Ferreira, – São Paulo: Platos Soluções Educacionais S.A., 2021.

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
