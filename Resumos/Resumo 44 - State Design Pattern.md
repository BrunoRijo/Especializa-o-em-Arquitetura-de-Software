# State Design Pattern
>[!Note]
>Resumo 44 | Especialização em Arquitetura de Software por Bruno Rijo

Opa!! O padrão de projeto state tem um entendimento bem simples, bora ver?

Permite que um objeto altere o seu comportamento quando o seu estado interno muda, e como ele faz isso? Evitando o uso de blocos de condicionais enormes baseados em estado, e trocando isso por objetos que representam cada estado.

Imaginando um problema do dia a dia, suponha que você trabalhe em um sistema de delivery onde os pedidos podem estar nos estados “Novo”, “Em preparo”, “Saiu para entrega”, “Entregue” e “Cancelado”, cada estado possui regras diferentes, tipo, “Em preparo” não pode ser cancelado, “Entregue” não pode ser alterado”.
Usando o padrão status, seria criado um objeto para cada estado e o pedido delega o comportamento atual ao objeto correspondente.

A estrutura desse padrão é composta por :
1. State (que pode ser Interface ou classe abstrata) - Declara os métodos que representam ações comuns a todos os estados.
2. ConcreteState -  Fornece suas próprias implementações para os métodos específicos dos estados declarados na interface State.
3. Context (Contexto) -  Possui um estado atual, e delega a ele um comportamento.
4. Cliente - Cria o contexto e manipula os estados.

No próximo resumo, falarei sobre o Interpreter.
Até o próximo.


[Lembrete] Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
