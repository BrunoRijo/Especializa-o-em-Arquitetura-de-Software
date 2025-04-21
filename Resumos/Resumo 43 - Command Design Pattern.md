# Command Design Pattern
>[!Note]
>Resumo 43 | Especialização em Arquitetura de Software por Bruno Rijo

Opa!! Seguimos com os padrões comportamentais. Dessa vez o Command.

O padrão de projeto Commando, tem como objetivo transformar uma requisição em um objeto independente que conterá todas as informações sobre essa requisição. Depois de transformar essa requisição em um objeto, ele desacopla quem solicitou de quem vai executar. 

Bora de analogia, imagine um controle remoto de TV, quando você aperta o botão de “ligar”, o controle não sabe exatamente como a TV se liga, ele só emite o comando, e a TV executa.

Suponha que você está criando um sistema de pedidos de uma lanchonete, e tem ações como “Criar Pedido”, “Cancelar Pedido” e “Notificar Cliente”. Ao invés de acoplar tudo em um método com if/else para cada ação, você cria comandos independentes com a mesma interface. Dessa forma, é possível criar filas de pedidos, implementar diferentes regras de negócios, adicionar logs e etc.

A estrutura básica é formada por:
1. Cliente - cria e configura objetos de requisições concretas, passando todos os parâmetros da requisição, incluindo uma instância do destinatário para o construtor da classe Command. Feito isso, a classe Commando irá resultar em um associado com múltiplos destinatários.
2. Classe Invoker (Remetente) responsável por iniciar as requisições, ela deve conter uma instância da classe command, irá acionar o comando ao invés de enviar a requisição diretamente para o destinatário.
3. Receiver (Destinatário) Contem a lógica de negócio, e quase qualquer objeto pode servir como um receiver, na maioria das vezes os comandos irão apenas lidar com os detalhes de como a requisição é passada para o receiver.
4. A classe ConcreteCommand, irá implementar vários tipos de requisição e passar a chamada para algum dos objetos da lógica de negócio.

No próximo resumo falarei sobre o padrão State.
Até lá. :) 

[Lembrete] Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

Fonte:
- Ferreira, Arthur Gonçalves. F383d - Design Patterns e gerência de configuração: do projeto ao controle de versões / Arthur Gonçalves Ferreira, – São Paulo: Platos Soluções Educacionais S.A., 2021.

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
