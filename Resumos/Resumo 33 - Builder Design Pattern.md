# Builder Design Pattern
>[!Note]
>Resumo 33 | Especialização em Arquitetura de Software por Bruno Rijo

Seguindo com os padrões criacionais, hoje vou falar um pouco sobre o Builder!!

Ele é um padrão utilizado para criar objetos complexos passo a passo, de maneira organizada e reutilizável. Ele separa a construção de um objeto de sua representação, permitindo criar diferentes representações do mesmo objeto utilizando o mesmo processo de construção.

Vou citar uma analogia pra deixar tudo mais fácil de entender, imagine que você quer montar um sanduíche, esse sanduíche pode ser simples com pão, presunto e queijo ou mais complexo, com alface, tomate, maionese, frango, bacon e outros ingredientes. O padrão Builder funcionaria como um manual de montagem desse sanduíche.

A classe builder teria um padrão de como se monta esse sanduíche, seguindo um passo a passo: primeiro o pão, depois os recheios, depois os molhos e assim por diante. Mas  o artifício principal desse padrão é que você pode pedir um sanduíche simples, ou cheio de ingredientes, ele sempre vai ser montado seguindo esse passo a passo, mas o resultado pode ser diferente.

Acho que já ficou bem claro o funcionamento, mas trazendo um pouco mais pra nossa realidade imagine que você precisa criar um relatório PDF que pode variar os campos que aparecem no cabeçalho, rodapé e o seu conteúdo. Com o padrão você teria os métodos addHeader, addFooter e addContent que teriam diferentes implementações para diferentes tipos de relatórios.

Algumas vantagens desse padrão são:
- Flexibilidade, para criar diferentes representações do mesmo objeto.
- Separação de responsabilidades, uma vez que o padrão isola o código de construção da lógica de negócios.
- Clean code, evita construtores complexos ou objetos com muitos parâmetros opcionais.

A Estrutura desse padrão contém:
1. A Classe Produto, que é o produto que será criado
2. A interface Builder define os passos necessários para construir o produto.
3. As classes concretas que implementam a interface builder e contém as implementações específicas para os passos definidos.
4. Uma classe para coordenar a criação do produto utilizando o builder, apesar de não ser obrigatória.

[Lembrete] Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles. Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

No próximo resumo vou falar sobre o Abstract Factory, até o próximo. :)

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
