# Abstract Factory Design Pattern
>[!Note]
>Resumo 34 | Especialização em Arquitetura de Software por Bruno Rijo

O padrão Abstract Factory é um padrão criacional que fornece uma interface para criar famílias de objetos relacionados ou dependentes sem especificar suas classes concretas. Ele permite que você crie objetos de forma flexível e organize-os em famílias.

Bora fazer uma analogia aqui, imagina que você é dono de uma rede de restaurantes. Em cada restaurante, você pode pedir um menu completo (entrada, prato principal e sobremesa) baseado na localização, por exemplo restaurante italiano, japonês ou libanês. Cada restaurante é como uma Abstract Factory que produz “famílias” de itens relacionados, no caso, um menu completo diferente em cada localização.

Uma dúvida que me apareceu enquanto estudava esse padrão foi, “Qual a diferença entre o Abstract Factory e o Factory Method?”. E de acordo com a minha pesquisa o Factory Method é mais simples pois ele delega a criação de um único objeto, ele define um método que as subclasses implementam para criar esse objeto. Já o Abstract Factory tem foco em criar FAMÍLIAS de objetos, ou seja, fornece uma interface que cria múltiplos tipos de objetos que pertencem a uma mesma família. E apesar de diferentes, ambos os padrões podem ser utilizados juntos, de modo que o Abstract Factory forneça a interface para criar as famílias de objetos, mas delegue a criação de cada objeto específico a um Factory Method.

Na vida real, imagine que você precise criar um sistema que deve ser compatível com vários bancos de dados diferentes. Cada banco de dados possui formas diferentes de criar conexões e executar consultas, o Abstract Factory ajudaria a manter o código do cliente consistente, sem se preocupar com os detalhes específicos de cada banco.

A estrutura do Abstract Factory, inclui:
1. Abstract Factory, que é a interface ou classe abstrata que declara os métodos para criar os diferentes produtos de uma família.
2. Classes concretas que implementam os métodos especificados na interface Abstract Factory.
3. Abstract Product, que define uma interface para um tipo de produto.
4. A Classe que implementa o Abstract Product e define um tipo específico de produto.
5. Client, que utiliza apenas as interfaces Abstract Factory e Abstract Product sem depender das classes concretas correspondentes.

No próximo resumo vou falar sobre o Prototype, até lá. :)

[Lembrete] Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
