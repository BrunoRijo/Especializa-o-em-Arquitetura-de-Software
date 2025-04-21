# Template Method Design Pattern
>[!Note]
>Resumo 48 | Especialização em Arquitetura de Software por Bruno Rijo

Ainda seguindo na sequência dos padrões comportamentais, falarei hoje sobre o Template Method.

O objetivo desse padrão é permitir que o desenvolvedor defina o fluxo de execução de um processo, mas deixe que partes específicas do comportamento sejam definidas pelas subclasses.

Um exemplo no dia a dia, bora lá, imagina que vc tem um sistema que possui uma função de importação de arquivos para CSV, JSON, XML .. e o processo é o seguinte: Validar o arquivo, ler os dados, processar os dados e salvar no banco. Esse processo vai ser sempre igual, independente do tipo de arquivo que vai ser importado.. mas a forma como os dados serão lidos e processados pode variar, então com o template method, vc criaria uma classe abstrata para fazer a importação, contendo todo o processo comum a todos os tipos, e para cada um deles, uma classe abstrata que faça sua parte da forma específica.

A estrutura para implementação é bem simples:
1. Abstract Class - Possui o método final que define o um fluxo padrão, e também outros métodos que podem já estar implementados ou serem abstratos.
2. Concrete Class - É uma subclasse que existe para sobrescrever todos os métodos abstratos definidos na Abstract Class.

Na sequência, vou falar sobre o padrão Mediador..

[Lembrete] Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

Referência:
- Design Patterns e gerência de configuração: do projeto ao controle de versões / Arthur Gonçalves Ferreira, – São Paulo: Platos Soluções Educacionais S.A., 2021.

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
