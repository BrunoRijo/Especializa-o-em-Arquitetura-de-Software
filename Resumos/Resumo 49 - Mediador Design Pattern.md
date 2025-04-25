# Mediador Design Pattern
>[!Note]
>Resumo 49 | Especialização em Arquitetura de Software por Bruno Rijo

Na reta final da saga dos padrões de projeto … vou falar sobre o padrão comportamental Mediador.

Basicamente, esse padrão encapsula a comunicação entre objetos, garantindo que os objetos não interajam diretamente. Cada objeto reconhece a um mediador central, e esse mediador atua fazendo o intermédio da comunicação, recebendo e repassando as requisições entre os objetos.

O objetivo é evitar pendências diretas entre objetos, e centralizar as regras de interação, facilitando a manutenção e evolução de código…

A estrutura da implementação, segue o seguinte padrão:
1. Interface Mediator - Declara os métodos de comunicação.
2. Concrete Mediator - Implementa a lógica de interação entre os objetos.
3. Colleague - Interface ou classe base dos componentes que se comunicam entre si, através do mediador.
4. Concrete Colleague - São os objetos que usam o mediador.

[Lembrete] Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

Referência:
- Design Patterns e gerência de configuração: do projeto ao controle de versões / Arthur Gonçalves Ferreira, – São Paulo: Platos Soluções Educacionais S.A., 2021.

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
