# Introdução a Computação em Nuvem
>[!Note]
>Resumo 20 | Especialização em Arquitetura de Software por Bruno Rijo

Esse assunto é particularmente especial para mim, porque foi tema do primeiro artigo que escrevi junto com um colega na época da faculdade, de lá pra cá esse assunto sempre aparece de alguma maneira pra mim haha.


Bora lá,

Historicamente, a computação pode ser dividida em 3 momentos principais

1. MainFrames -  Na década de 1960, a computação era utilizada basicamente com o uso de mainframes, que eram computadores gigantes localizados em grandes corporações ou Instituições governamentais. Por serem o que havia de mais avançado na época em termos de capacidade computacional, os clientes precisavam ir pessoalmente ao local onde esses mainframes estavam para utiliza-los.

2. Cliente/Servidor - Na década de 1980, surgiu o paradigma Cliente-Servidor, onde um computador relativamente pequeno dispõe de serviços que podem ser utilizados por vários clientes espalhados geograficamente, conectados por uma rede.

3.Cloud, surgida a partir dos anos 2000, nesse conceito os dados sao armazenados em locais chamados Data Centers, onde diversos clientes ao redor do mundo, conectados através da internet conseguem acessar esses recursos para atender as suas demandas.

O primeiro grande conceito que precisa ser compreendido na arquitetura de nuvem é o Cloud.

Os serviços são fornecidos para os usuários através da nuvem, como AWS, Google Cloud, IBM, diversas empresas oferecem aplicações pra oos usuários, e são mais comuns do que percebemos as vezes, e fazem parte do nosso dia a dia como as redes sociais ou o youtube.

A arquitetura da nuvem consiste em dois elementos principais, os componentes da arquitetura e as conexões/interções entre esses componentes.

Os componentes, são os elementos que compoem a infraestrutura da nuvem, podem ser Servidores, Dispositivos de armazenamento, Interfaces de rede, Clusters, Sistemas operacionais e etc.

É importante sabet que Arquitetura é diferente de Infraestrutura, enquanto a arquitetura diz respeito aos componentes e a interconexão entre eles, a infraestrutura se refere apenas aos componentes em si.

Um dos principais componentes é o datacenter, é o local onde a nuvem é implementada, é o local que recebe as requisiões dos usuários, e provê os dados conforme as solicitações.

um datacenter  é composto por elementos de:

- Processamento (Servidores)
- Armazenamento (Discos, Storages)
- Comunicação (Interfaces de rede, hubs, switches)
- Software (SO, Middleware, virtualização e etc)

Uma das principais tecnologias para habilitar a CP em um datacenter é a virtualização, que é um processo de desacoplamento da estrutura física das aplicações, ou seja, quando uma aplicação vai fazer uma requisição na nuvem, a aplicação requisita um recurso virtual, que é então mapeado para um recurso físico. Cada máquina virtual pode oferecer um servidor virtual que possua o SO definido pela aplicação, que acessa o datacenter e busca os dados requisitados.

A Arquitetura de Nuvem pode ser organizada em camadas.

Na camada mais baixa, temos os servidores físicos que vão realizar o processamento.
Acima dessa camada, teremos a de virtualização que vai ocultar a infraestrutura fisica das aplicações e oferecer recursos virtualizados na nuvem.
Acima dessa camada temos a camada de bancos de dados
e pro fim a camada de aplicação.

Os modelos de serviço na nuvem são

Iaas (Infraestrutura as a Service), é um serviço que oferece aos usuários os recursos da infraestrutura virtualizada, pode oferecer servidores, dispositivos de armazenamentos, SSD, HDD, sistemas de arquivos compartilhados, discos, virtualização e etc …

Paas (Platafrma como Serviço), diferente do Iaas, o Paas ferece plataformas de ferenciamendo dos recursos na nuvem , como SO’s, sistemas de middleware que são software que atuam entre as estruturas fisicas e as aplicações, são utilizados para fornecer funcionalidades básicas da computção na nuvem, Exemplo: Firewall.

Saas (Software como Serviço), por ultimo, esse modelo corresponde a uma aplicação pronta que é oferecida ao usuário, exemplo: redes sociais, ferramentas de edição de documentos e etc … 

Lembrando que o Saas não é a Nuvem, o Saas é uma aplicação pronta oferecida ao usuário, enquanto a nuvem diz respeito a todos os recursos, e serviços que a nuvem pode oferecer.

Até a próxima. 🙂

Caso queira ver tudo outros resumos que já produzi, basta visitar meu perfil no github: https://lnkd.in/dqCG6wqj

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware
