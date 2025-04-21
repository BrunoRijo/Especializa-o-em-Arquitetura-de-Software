# Memento Design Pattern
>[!Note]
>Resumo 42 | Especialização em Arquitetura de Software por Bruno Rijo

Opa!! tudo bem? Seguindo a saga dos resumos, vou falar hoje sobre um que permite salvar os estados de um objeto, o Memento.

Esse padrão de projeto é bem legal, ele permite que se salve e restaure estados de determinado objeto sem ser necessário revelar os detalhes desta implementação. É ideal quando você precisa de uma opção de “desfazer” algo, ou criar checkpoints em objetos. É tipo um Control + Z.

A estrutura dele é formada por:
1. Caretaker-  controla quando e porque o estado da classe originator deve ser capturado ou guardado.
2. Originator (Originador) - armazena os estados em uma pilha, quando for necessário recuperar  um estado a classe caretaker irá buscar o estado requisitado na classe originator e passar para o método de restauração. Essa classe permite criar estados de si mesma e restaurar quando necessário.
3. Memento - Armazena, de fato, a estrutura do estado.

Uma grande vantagem desse padrão é a facilidade de implementação e por ser bem útil em sistemas que precisam de rollback em operações. Já a maior desvantagem que encontrei sobre esse padrão é o grande uso de memória que pode ser utilizado se forem salvos muitos estados, além de que se o objeto for complexo, pode haver também um custo de performance.

Até o próximo resumo.

[Lembrete] Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

Fonte:
- Ferreira, Arthur Gonçalves. F383d - Design Patterns e gerência de configuração: do projeto ao controle de versões / Arthur Gonçalves Ferreira, – São Paulo: Platos Soluções Educacionais S.A., 2021.

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
