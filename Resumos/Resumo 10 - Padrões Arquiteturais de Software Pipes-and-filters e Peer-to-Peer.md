# Padrões Arquiteturais de Software Pipes-and-filters e Peer-to-Peer
>[!Note]
>Resumo 45, Especialização em Eng. de Software por Bruno Rijo

## Arquitetura Pipes-and-filters (PF) 👨‍🏭 
Nesse modelo arquitetural a funcionalidade de um sistema é organizada como uma série de componentes independentes chamados "filtros". Esses filtros processam dados e os transmitem para o próximo filtro através de "pipes" (tubos), formando uma cadeia ou pipeline. É mais utilizado em aplicações que necessitam de processamento sequencial de dados, como sistemas de áudio, vídeo ou dados em lote.

Os filtros (filters) são unidades de processamento independentes que recebem dados de entrada, processam esses dados e produzem uma saída. Cada filtro faz uma operação específica, como transformar, filtrar ou agregar dados..

Já os tubos (pipes), conectam os filtros, transmitindo a saída de um filtro como entrada para o próximo. Eles são responsáveis por mover os dados entre os componentes.

**Exemplo**:
Suponha que você trabalhe em  um sistema de processamento de imagem, um filtro pode aplicar um efeito de brilho a uma imagem. Nesse caso, haverá um pipe que passa a imagem pelo filtro de brilho para o usuário aplicar outros filtros, caso deseje.

**Vantagens** 👍
- Modularidade: Filtros são independentes e podem ser adicionados, removidos ou substituídos facilmente.
- Reusabilidade: Filtros podem ser reutilizados em diferentes pipelines ou sistemas.

**Desvantagens** 👎
- Desempenho: Em casos de sobrecarga no pipe.
- Complexidade na Gestão de Estado: Manter o estado entre filtros pode ser complicado, especialmente se os filtros forem projetados para serem completamente independentes.


## Arquitetura Peer-to-Peer (P2P) 👥 
Esse modelo é um espécie de rede onde cada participante, ou "peer" (par), tem capacidades e responsabilidades iguais, agindo tanto como cliente quanto como servidor. Não há uma hierarquia central, e todos os peers podem se comunicar diretamente entre si. É bastante usado em aplicações com compartilhamento simultâneo de arquivos, redes de comunicação, como skype.

Como citei anteriormente, cada Peer pode enviar e receber dados, compartilhar recursos ou serviços, e colaborar com outros peers na rede. A rede não depende de um servidor centralizado, todos os peers participam da manutenção da rede, compartilhando a carga de trabalho e dados.

**Vantagens** 👍
- Escalabilidade: A rede pode crescer facilmente à medida que novos peers entram, sem a necessidade de um servidor centralizado.
- Custo Reduzido: Não há necessidade de investir em servidores centralizados caros, já que os próprios peers fornecem os recursos.

**Desvantagens** 👎 
- Segurança: A ausência de um controle centralizado pode dificultar a implementação de medidas de segurança, tornando a rede vulnerável a ataques.
- Complexidade na Sincronização: Manter os dados sincronizados entre vários peers, em redes grandes, pode ser complicado.

Essa é foi uma repostagem de um resumo já produzido por mim, durante essa mesma cadeira no curso de [Especialização em Engenharia de Software](https://github.com/BrunoRijo/Especializa-o-em-Engenharia-de-Software).

Até o próximo! 🤗
