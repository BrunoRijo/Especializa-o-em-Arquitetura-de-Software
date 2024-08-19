# Principais estilos e padrões Arquiteturais de Software 
>[!Note]
>Resumo 08, Especialização em Arquitetura de Software por Bruno Rijo

A escolha de uma arquitetura resultará no atendimento a aspectos como a performance, qualidade, facilidade de manutenção e escalabilidade. Portanto, essa decisão resulta em impacto no sucesso ou insucesso do projeto, especialmente a longo prazo (SILVEIRA et al., 2011). 

Cada decisão e solução a ser criada requer um determinado tipo de arquitetura, para auxiliar nas escolhas, alguns estilos e padrões arquiteturais foram, com base em sua utilização na indústria e academia, estabelecidos. A seguir tais padrões são apresentados e discutidos (SILVEIRA et al., 2011; PRESSMAN, 2021, SOMMERVILLE, 2018).

## Arquitetura em Camadas 📚📚 
É uma forma de organizar um sistema em níveis distintos, onde cada camada tem uma função específica e interagem apenas com a camada adjacente. 

Vou citar aqui as camadas dando um exemplo simples, imagine um aplicativo de pedidos de comida:

1️⃣ 📱 **Camada de apresentação**
Interface do usuário, onde você vê o menu e faz o pedido.

2️⃣ ⚙ **Camada de lógica de negócio**
Processa o pedido, calcula o total e verifica a disponibilidade

3️⃣ 🔗 **Camada de persistência**
Lida com a forma como os dados são persistidos.

4️⃣ 🗄️ **Camada de Dados**
Armazena informações sobre o cardápio, pedidos e usuários.

**Vantagens** 👍 
- Modularidade, cada camada pode ser desenvolvida e modificada separadamente.
- Reusabilidade, componentes de uma camada podem ser reutilizados em outros sistemas.

**Desvantagens** 👎 
- Desempenho, a comunicação em camadas pode gerar sobrecarga e reduzir a performance
- Complexidade, pode adicionar complexidade desnecessário em sistemas simples.


## Arquitetura cliente-servidor (client-server) 👨‍💻🗄️ 
É uma arquitetura na qual o processamento da informação é dividido em módulos ou processos distintos. Existe um processo que é responsável pela manutenção da informação (servidor) e outro responsável pela obtenção dos dados (os clientes).

Um cliente solicita um determinado serviço, através do envio de uma mensagem ao servidor. Enquanto o processo servidor está trabalhando a solicitação, o cliente está livre para realizar outras tarefas.

Um Servidor oferece serviços a processos usuários, ou seja, executam a tarefa solicitada e enviam uma resposta ao cliente que se traduz nos dados solicitados.

**Vantagem** 👍 
- Recursos centralizados
- Facilidade de manutenção

**Desvantagem** 👎 
- Sobrecarga, o servidor pode ficar sobrecarregado caso receba mais solicitações o que suporta
- Único nó, se um servidor crítico falha, os pedidos dos clientes não podem ser cumpridos por centralizar todas as solicitações em um único ponto.

Tem vários outros modelos de arquitetura, vou trazer mais alguns deles no resumo 09!!

Se você leu até aqui, comenta se você já usou algum modelo arquitetural desses ou qual(is) você utiliza nos seus projetos ??

Essa é foi uma repostagem de um resumo já produzido por mim, durante essa mesma cadeira no curso de [Especialização em Engenharia de Software](https://github.com/BrunoRijo/Especializa-o-em-Engenharia-de-Software).

Até o proximo!! 🙂
