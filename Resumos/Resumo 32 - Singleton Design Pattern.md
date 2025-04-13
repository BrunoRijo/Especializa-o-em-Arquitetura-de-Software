# Singleton Design Pattern
>[!Note]
>Resumo 32 | Especialização em Arquitetura de Software por Bruno Rijo

Eu pessoalmente acredito que esse é o padrão mais conhecido e utilizado dentre todos, tanto pela sua simplicidade de entendimento e de implemetação.

O Padrão Singleton, propõe a criação de uma ÚNICA instância global para utilização de uma classe, e um ponto global de acesso dessa instância. Alguns exemplos de quando seria necessário utilizar esse padrão seriam em classes de conexão com banco de dados, gerenciadores de configuração ou até mesmo classes de log em sistemas que têm log centralizado.

Imagine um sistema que carrega configurações (como idioma, tema ou URLs de API). Usar um Singleton garante que todos o código acesse a mesma instância da classe de configurações, evitando inconsistências e carregamentos repetitivos.

A implementação desse padrão segue a seguinte estrutura:
- Construtor Privado: Que impede a criação direta de objetos.
- Atributo estático da própria classe: Que armazena a única instância da classe.
- Método estático público: Que retorna a instância única, criando-a se ainda não existir.

As vantagens de utilizar o padrão singleton são:
1. Permite que as operações sejam mais flexíveis do que as realizadas entre classes.
2. Não é necessário se preocupar em controlar as instâncias de classe.
3. As operações ficam mais refinadas.
4. Instâncias únicas, por classe.

[Lembrete]
Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

No próximo resumo vou falar sobre o Builder, até lá. :)

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
