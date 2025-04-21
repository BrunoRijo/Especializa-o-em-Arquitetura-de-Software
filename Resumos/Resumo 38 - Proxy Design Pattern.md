# Proxy Design Pattern
>[!Note]
>Resumo 38 | Especialização em Arquitetura de Software por Bruno Rijo

Seguindo falando sobre os padrões de projeto estruturais, vou falar hoje sobre o Proxy!!

O objetivo deste design pattern é controlar o acesso a um objeto real (ou real subject), através de um substituto ou representante, o proxy. A gente pode pensar no proxy como um intermediário inteligente que age como se fosse o objeto real, mas pode fazer coisas extras antes ou depois de delegar a chamada para o objeto real.

Um exemplo, imagine que você trabalha com um sistema que manipule arquivos muito grandes de video. A classe “Video” carrega os dados completos do vídeo, o que pode ficar pesado. Nesse caso, você pode criar um proxy chamado “VideoProxy” que só carrega o vídeo real quando o usuário clicar em “play”. Assim, a interface do sistema pode listar 100 vídeos com informações básicas sem travar ou demorar para abrir a página.

Tem outras situações em que o Proxy pode ser utilizado, por exemplo, para realizar autenticação antes de acessar o objeto real, guardar cache de dados ou realizar consultas complexas, fazer comunicação com API’s externas e até mesmo registrar logs de acesso ou de monitoramento.

Tem algumas vantagens que podem ser listadas sobre esse padrão, como:
- Melhoria de performance (em casos de adiar o carregamento de instâncias pesadas, como no exemplo que dei acima).
- Responsabilidade única, pois o Proxy pode ficar responsável por cuidar de coisas como log, cache e autenticação.
- Encapsulamento de complexidade, pois o cliente nem sabe que vai estar falando com um proxy.

A estrutura da implementação é composta por:
- Subject (Interface comum) - declara uma interface que deverá ser seguida tanto pelo proxy quanto pelo objeto real.
- Real Subject (Objeto Real) - que contém a lógica da funcionalidade.
- Proxy - que contém uma referência ao objeto real e adiciona funcionalidades intermediárias.

Essa é a ideia do proxy, espero ter sido claro :) se ficar alguma dúvida pode comentar aqui embaixo.

[Lembrete] Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

Fontes:
- Ferreira, Arthur Gonçalves. F383d - Design Patterns e gerência de configuração: do projeto ao controle de versões / Arthur Gonçalves Ferreira, – São Paulo: Platos Soluções Educacionais S.A., 2021.

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
