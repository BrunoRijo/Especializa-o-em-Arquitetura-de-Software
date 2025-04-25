# Visitor Design Pattern
>[!Note]
>Resumo 50 | Especialização em Arquitetura de Software por Bruno Rijo

Chegando ao fim da saga dos padrões de projeto kkk finalmenteeee.

O último padrão que vou citar aqui, é do tipo comportamental, e é chamado de Visitor,a chei bem interessante.

O objetivo dele é separar operações específicas da estrutura, permitindo adicionar essas operações a uma estrutura de objetos sem precisar modificar suas classes. Ele desacopla os algoritmos dos objetos sobre os quais eles operam. Em outras palavras, ele “visita” os objetos com uma lógica externa, sem mudar o objeto em si.

Imagina que você atue em um sistema de editor gráfico, com várias formas (circulo, retângulo, linha, etc). E você precisa implementar exportação para PNG, impressão e alguma outra funcionalidade nova. Se você adicionar tudo isso nas classes das formas, vai ter um código poluído e repetitivo. Nesse caso, você poderia usar o Visitor, e criar “visitantes” para essas operações, e as formas só precisariam aceitar esses visitantes.

Entre as vantagens estão
- Adicionar novas operações sem modificar a estrutura dos objetos
- Separação de responsabilidades

Já como desvantagem
Pode ser verboso já que cria muitas classes e métodos ..
Não lida bem com mudanças frequentes de hierarquia de objetos

A estrutura para implementação é a seguinte:
1. nterface Element - Declara um método para aceitar visitantes.
2. Concrete Element - Implementa os métodos que aceitam os visitantes.
3. Interface Visitor - Declara um método visit() para cada tipo concreto de elemento.
4. Concrete visitor - Implementa as operações específicas que são aplicadas a cada elemento.

Com isso finalizo a cadeira de Design Patterns.

No próximo resumo, iniciarei outra cadeira super interessante da minha pós que é sobre API’s e Webservice.

até lá :)
