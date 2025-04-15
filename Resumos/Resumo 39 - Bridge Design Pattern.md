# Bridge Design Pattern
>[!Note]
>Resumo 39 | Especialização em Arquitetura de Software por Bruno Rijo

Opa, tudo bem? Vou falar hoje sobre o padrão Bridge!!

O Bridge tem como objetivo separar a abstração da implementação, permitindo que as duas evoluam independentemente. Normalmente esses dois elementos estão presos um ao outro, o bridge separa os dois, e coloca uma ponte entre eles. Ele pode ser usado quando
você precisar trocar a implementação em tempo de execução e quer evitar a criação de várias classes com a mesma implementação.

Para entender melhor, imagine vc está desenvolvendo um sistema de notificações. Você tem diferentes tipos de notificação (Alerta, Confirmação, Promoção) e diferentes canais de envio (Email, SMS) se vc usar uma herança direta teria que criar várias combinações entre cada tipo de notificação e cada tipo de envio, exemplo: AlertaViaEmail, AlertaViaSMS, ConfirmacaoViaEmail .. etc.
Isso criaria um emaranhado de classes bem grandinho…
Para resolver isso, você separaria a abstração criando uma interface para Notificação, e implementando uma classe que segue essa interface e envia uma mensagem de acordo com o canal de envio desejado. E a implementação no caso, seria criar uma interface para o canal de envio, e as classes de canais que implementam suas particularidades.
O padrão bridge conectaria ambos. A notificação escolhe “como” enviar, sem se preocupar com “quem” vai enviar, criando o canal de comunicação, e a notificação que agirá de acordo com esse canal criado em tempo de execução.

Apesar de ser um pouco difícil de entender no início, esse padrão pode ajudar na manutenção e evolução do sistema além de reduzir a explosão de subclasses.

A estrutura básica é composta por:
1. Abstraction (Abstração) - é a camada de mais alto nível, visível para o cliente. Mantém uma referência para a implementação.
2. RefinedAbstraction - é uma versão concreta da abstração.
3. Implementor (Implementação) - declara uma interface comum a todas as implementações concretas, essa abstração só pode se comunicar a um objeto de implementação por métodos declarados fora dessa classe.
4. ConcreteImplementor - contém as implementações reais.

No próximo resumo vou falar sobre o Chain of Responsability.
