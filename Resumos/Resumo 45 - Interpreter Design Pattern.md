# Interpreter Design Pattern
>[!Note]
> Resumo 45 | Especialização em Arquitetura de Software por Bruno Rijo

Opa!! bom dia!!

O padrão Interpreter, segundo minhas pesquisas, é um dos menos usados no dia a dia, maaasss, pode ser útil quando se precisa interpretar linguagens ou expressões com estrutura repetitiva, como fórmulas, comandos ou filtros.

Ele é um padrão do tipo comportamental, que define uma gramática para uma linguagem e usa uma estrutura de classes para interpretar as sentenças dessa linguagem. Seria como um mini interpretador para comandos ou expressões, geralmente construído em estruturas de árvores.

Possui basicamente 5 classes
1. AbstractExpression (Pode ser uma interface ou uma classe abstrata) - Define a operação de interpretação comum a todas as expressões.
2. Terminal Expression - Representa expressões independentes, básicas, sem nenhuma subexpressão.
3. NonTerminalExpression - Combina expressões usando operadores (e/ou/etc)
5. Context (Contexto) -  Representa os dados inseridos, processados e resultantes. Geralmente vai possuir uma variável de entrada a uma de saída.

[Lembrete] Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
