# Funções dos Atores na Nuvem e SLA.
>[!Note]
>Resumo 24 | Especialização em Arquitetura de Software por Bruno Rijo

Em um ecossistema de nuvem existem três atores principais: O provedor de serviços, o usuário e o desenvolvedor da aplicação.

O provedor de serviços é quem implementa e fornece os serviços para os demais atores, oferecendo Iaas, Paas e Saas.
O Desenvolvedor de aplicação irá consumir o serviços de infraestrutura e de plataforma, e fornecer serviços de software que serão consumidos pelos usuários.
Enquanto o usuário apenas consome os serviços de software já prontos.

O Acordo a nível de serviço ou SLA, é um contrato estabelecido entre duas partes, que possui o seguinte ciclo de vida.
1. O usuário descobre qual o provedor de serviço que melhor atende às suas necessidades
2. Definir qual9is) os SLA’s que necessita
3. Estabelecer um acordo
4. Monitorar violação do SLA.
5. Caso algum SLA seja violado, então o cliente termina o SLA
6. Forçar penalidades sobre o SLA.

O SLA, ou Service Level Agreement, ou Acordo de nível de serviço, pode ser sob demanda ou reservado.

No modelo sob demanda, o usuário estabelece um contrato com o provedor sob um curto período de tempo, enquanto o usuário utiliza o serviço o SLA está valendo, caso o cliente utilize somente 1 hora por dia, então o SLA irá cobrar somente 1 hora de uso. Já o modelo reservado, o contrato é feito por um prazo mais longo, exemplo, se o cliente contratar o SLA por um 1 mês, então ele utilizando ou não o serviço será cobrado.

Qualquer regra de interesse pode ser incluída dentro o SLA, uma vez que diga respeito ao desempenho do sistema ou gerenciamento de problemas, o SLA também deve conter as penalidades para ambas as partes envolvidas caso haja alguma violação de regra.

Até o próximo. :)

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
