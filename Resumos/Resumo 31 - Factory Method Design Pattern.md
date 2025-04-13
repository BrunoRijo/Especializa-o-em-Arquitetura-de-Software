# Factory Method Design Pattern
>[!Note]
>Resumo 31 | Especialização em Arquitetura de Software por Bruno Rijo

Iniciando uma parte bem legal dos resumos, na verdade acho que fiz essa pós só por causa dessa cadeira kkk vou falar sobre todos os padrões de projeto, começando pelos de criação, o primeiro será o Factory Method.

O Factory Method é um padrão que permite que se produza famílias de objetos relacionados sem precisar especificar suas classes concretas. Em vez de se criar diretamente o objeto, você delega essa tarefa a um objeto chamado factory (Fábrica).

Imagine que você esteja implementando um sistema para processar pagamentos, em diferentes métodos como cartão de crédito, pix, boleto bancário e etc. Cada método de pagamento precisa de uma implementação diferente (acessar APIs específicas, validar informações, etc). Ao invés de criar os objetos de pagamento diretamente no seu código principal, você pode usar o Factory Method para delegar a criação do objeto do tipo correto de pagamento a classes específicas sem que o código principal precise saber os detalhes de implementação de cada um.

Esse padrão é composto por basicamente 5 elementos:

1. Uma interface que será responsável por declarar um conjunto de métodos para cada um dos produtos abstratos.
2. As Classes Concretas que são a implementam a interface e os seus métodos.
3. Classe factory, que é de fato a fábrica e o centro desse pdrão de projeto, ela será uma classe abstrata que possui um método abstrato create, que será sobrescrito pelas classes responsáveis pela criação de objeto de cada uma das classes concreta, e que implementa os métodos necessários utilizando um objeto genérico.
4. Classes que herdam da factory e sobrescrevem o método abstrato de criação, retornando o objeto criado com seu tipo concreto correspondente.
5. A classe que será responsável pela criação do factory e passando a configuração correspondente para a criação correta, sem que nada precise ficar explícito.

Eu pretendo trazer a implementação de todos os padrões, ao fim dos resumos, e iniciar uma nova série de postagens com a implementação de cada um deles.
Enquanto isso, vou seguir tentando trazer a teoria da maneira mais clara possível nessa série aqui.

No próximo resumo vou falar sobre o Singleton, até lá. :)

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
