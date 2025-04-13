# Composite Design Pattern
>[!Note]
>Resumo 37 | Especialização em Arquitetura de Software por Bruno Rijo

O  Composite é um padrão do tipo estrutural.

Ele é baseado em uma estrutura de árvore onde os nós podem ser tanto objetos individuais (folhas) quanto grupos de objetos (compósitos). O objetivo é permitir que o cliente interaja com os objetos da árvore individualmente, sem precisar se preocupar se está lidando com uma folha ou com um grupo de elementos.

A estrutura do Composite envolve:
1. Component: Interface comum para todos os objetos na composição. Define operações que podem ser aplicadas tanto a folhas quanto a compósitos.
2. Leaf (Folha): Implementação concreta de um elemento que não possui filhos. Representa um objeto individual.
3. Composite: Implementação concreta que armazena filhos e delega chamadas para eles.
4. Client: Interage com os objetos sem precisar distinguir se são folhas ou compósitos.

Pra entender melhor o funcionamento desse padrão, imagine um módulo no seu sistema que seja responsável pelo gerenciamento de permissões. Um usuário pode ter permissões individuais ou fazer parte de um grupo que herda permissões de outros grupos.As permissões individuais seriam representadas nesse padrão como as folhas, e as permissões de grupos de usuários seriam os compósitos.

As vantagens de uso do composite basicamente são a facilidade de manipulação, uma vez que o padrão permite tratar elementos individuais ou grupos de elementos da mesma maneira, e a flexibilidade na hierarquia dos objetos, podendo adicionar, remover ou manipular objetos sem impactar na estrutura.

Já como desvantagens vou citar a complexidade, pois implementar essa padrão pode ser mais trabalhoso do que lidar com estruturas mais simples como listas, além de que muitas eles vezes ele pode ser desnecessário.

Esse foi um resumo sobre o composite, no próximo vou falar sobre o Proxy

[Lembrete] Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
