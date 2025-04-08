# IoT
>[!Note]
>Resumo 26 | Especialização em Arquitetura de Software por Bruno Rijo

## O que é o IoT?
Internet of Things, ou Internet das coisas, diz respeito ao conceito de que qualquer coisa pode se comunicar com qualquer coisa ou pessoa, através da internet.

6 tecnologias que são necessárias para habilitar o paradigma de Internet das coisas, são elas: Serviços, Identificação dos dispositivos, Sensoriamento, Semântica, Comunicação e Computação.

### A estrutura arquitetural do funcionamento da IoT pode ser representada por 5 camadas:

Na camada mais inferior estão os dispositivos, que são a fonte de dados e entidades físicas que interagem com o ambiente, como carros, telefones, eletrodomésticos etc .. Nessa camada os dispositivos trocam dados entre si, e também com a rede, utilizando a segunda camada que é a de “comunicação”.

A camada de comunicação, os dados são trafegados por meios de mensagens de comunicação e agregados por dispositivos intermediários que podem ser roteadores, provedores de internet, que compõem a terceira camada.

Através dos dispositivos intermediários, os dados chegam a próxima camada que é responsável pela análise e processamento de eventos, essa é a camada que representa a nuvem.

Estando na nuvem os dados servirão para alimentar os componentes da última camada que são os dispositivos de WEB, Dashboards, Gerenciamento de APIs ... qualquer item que consuma os dados inseridos na nuvem.

## Computação de Borda!
Como mencionei anteriormente, existem dispositivos intermediários entre os dispositivos da IoT e a Nuvem, foi notado que por vezes, pode existir um problema de envio de dados dos dispositivos até a nuvem, o tempo de resposta, ou latência pode ser muito alto, logo, foi criado o paradigma de computação de borda que faz com que alguns serviços que antes eram executados em nuvem, serem executados nos dispositivos da segunda camada, enviando para a nuvem somente os serviços que precisam de grande capacidade computacional.

O oferecimento de serviços de BD para os usuários, configura o modelo DBaaS, que visa fornecer serviços de BD específicos para os usuários. Composta por Infraestrutura física, um hypervisor e máquinas virtuais que serão disponibilizadas para os clientes, contendo apenas o acesso aos bancos. Para que um serviço seja disponibilizado pela nuvem é necessário que a nuvem disponha um serviço de monitoramento de DB que mede e avalia o desempenho dos demais dispositivos da arquitetura, os parâmetros de desempenho observados garantem métricas de confiabilidade, consumo de energia, parâmetros de segurança, capacidade de atender ao SLA e etc.

Até o próximo resumo!!. :)

Para ver a lista completa com todos os resumos que já produzi do meu curso de Arquitetura de Software, é só visitar o meu github. Segue o link: https://github.com/BrunoRijo/Especializa-o-em-Arquitetura-de-Software

#SoftwareEngineer #SoftwareArchitecture #EngenhariaDeSoftware #ArquiteturadeSoftware #SoftwareDeveloper
