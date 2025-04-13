# Adapter Design Pattern
>[!Note]
>Resumo 36 | Especialização em Arquitetura de Software por Bruno Rijo

Particularmente eu achei esse padrão bem interessante, principalmente para se usar em algumas situações de sistemas legados, onde já se tem uma estrutura funcionando e é necessário adicionar alguma nova funcionalidade.

O padrão de projeto Adapter ou Adaptador, garante a reutilização de código de uma interface específica de uma aplicação, atuando como um adaptador entre duas interfaces incompatíveis, permitindo que elas possam trabalhar juntas sem a necessidade de modificar o código já existente. Basicamente, esse padrão converte a interface de uma classe em outra interface que o cliente espera.

Por exemplo, imagine que você se depara com uma aplicação feita, a princípio, para usar JSON, e que agora você precisa adicionar suporte a arquivos XML, sem alterar o código já existente. Nesse caso, a biblioteca de leitura de XML tem uma interface diferente da usada para JSON,  e você poderia criar um adaptador para que a biblioteca de XML seja compatível com a interface esperada pelo sistema

Outro exemplo de uso real seria um sistema que precise enviar notificações para os usuários, mas cada provedor (E-mail, SMS, ou push) possui sua própria API com interfaces distintas. O seu sistema já possui uma interface comum para envio de notificações, e voce vai precisar adicionar suporte a um novo provedor, mas sem alterar o código cliente. A API de um novo provedor possui métodos e parâmetros que não seguem o padrão esperado pelo seu sistema, nesse caso você criaria um adapter para converter essa nova API para o modelo que o seu sistema já utiliza.

A estrutura básica do adapter possui 4 elementos, são eles:
1. Target (ou Alvo), que seria a interface esperada pelo cliente.
2. Adaptee (ou Adaptado) seria a classe ou componente existente com a interface incompatível, é o elemento que será adaptado.
3. Adatper (ou Adaptador), é uma classe que mplementa a interface Target e encapsula o objeto Adaptee, ele traduz as chamadas feitas para os métodos esperados pelo Adaptee.
4. Cliente, que é a classe que interage com o sistema por feiop da interface Target, sem conhecer os detalhes da implementação.

No próximo, falarei sobre o padrão Composite.

[Lembrete] Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper   
