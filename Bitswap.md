# Bitswap

>"*O Bitswap é um componente crucial na arquitetura do IPFS, possibilitando a troca eficiente de blocos de dados entre nós na rede descentralizada. Inspirado pelo protocolo BitTorrent, o Bitswap permite que os nós compartilhem listas de desejos e blocos de dados, evitando redundâncias e otimizando a transmissão e taxa de transferência. Ele também implementa um sistema de priorização inteligente e mecanismos para promover a equidade na rede.*"

O Bitswap é um componente crucial na arquitetura do InterPlanetary File System (IPFS), permitindo que ele funcione como um sistema de arquivos descentralizado e distribuído. Inspirado pelo protocolo BitTorrent, o Bitswap é, essencialmente, o mecanismo que permite a troca de blocos de dados entre nós da rede IPFS.

A operação do Bitswap é baseada em mensagens. Os nós na rede comunicam-se enviando mensagens uns aos outros, contendo "listas de desejos" (wantlists) e blocos de dados. A lista de desejos de um nó é simplesmente uma coleção de blocos de dados que ele está procurando. Quando um nó recebe uma lista de desejos de outro, ele verifica se possui algum dos blocos solicitados e, se tiver, envia-os para o nó solicitante.

Um aspecto distintivo do Bitswap é que ele é otimizado para evitar a redundância. Quando um nó recebe um bloco que estava em sua lista de desejos, ele emite uma mensagem de "cancelar" (cancel) para os outros nós, informando que ele já obteve o bloco e que não precisa mais dele. Isso evita que múltiplos nós enviem o mesmo bloco e, portanto, economiza recursos de rede.

O protocolo Bitswap também implementa um sistema de priorização inteligente. Ele permite que um nó atribua diferentes níveis de prioridade a diferentes blocos em sua lista de desejos. Isso pode ser útil em uma variedade de situações, por exemplo, se um nó está baixando vários arquivos simultaneamente, ele pode optar por priorizar blocos de um arquivo sobre os outros.

Outra funcionalidade do Bitswap é o sistema de "dívida", projetado para promover a equidade na rede. Quando um nó recebe um bloco de outro, ele "deve" a esse nó e é mais provável que responda aos futuros pedidos desse nó. Isso incentiva todos os nós a contribuir ativamente para a rede, compartilhando os blocos de dados que possuem, ao invés de apenas consumir recursos.

O Bitswap foi projetado para otimizar a capacidade de transmissão e a taxa de transferência da rede. Sua abordagem seletiva para a transmissão de blocos - transmitindo apenas os blocos que foram explicitamente solicitados - minimiza o consumo desnecessário de recursos e garante uma distribuição eficiente de dados.

Além disso, é importante destacar que, embora o Bitswap seja inspirado pelo BitTorrent, existem algumas diferenças cruciais. Em particular, o Bitswap não é um protocolo de compartilhamento de arquivos; é um protocolo de troca de blocos. Isso permite que blocos sejam obtidos de qualquer nó na rede que os possua, não importa onde o arquivo original foi obtido. Essa característica ajuda a aumentar a resiliência da rede IPFS, tornando-a mais robusta e descentralizada.

Junto com outros protocolos como o DHT (Distributed Hash Table) para localização de blocos e o IPLD (InterPlanetary Linked Data) para a interligação de blocos, o Bitswap ajuda a fornecer a base para o IPFS como um sistema de arquivos distribuídos eficiente e robusto.

Além disso, é essencial reconhecer que a implementação e o desenvolvimento do Bitswap estão em constante evolução, assim como o próprio IPFS. A comunidade de desenvolvedores está sempre buscando maneiras de melhorar a eficiência, a robustez e a escalabilidade do protocolo, tornando-o uma peça essencial do ecossistema de tecnologia de dados descentralizada.
