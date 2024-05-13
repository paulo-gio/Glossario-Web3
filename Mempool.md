# Mempool (Pool de Memória)

>"*O Mempool, ou Pool de Memória, é uma "área de espera" para transações de criptomoedas não confirmadas. Quando uma transação é iniciada, ela é verificada e, se válida, adicionada ao Mempool de cada nó da rede blockchain. Mineradores pegam transações deste pool para incluí-las em novos blocos, priorizando frequentemente aquelas com taxas mais altas. O estado do Mempool pode indicar o congestionamento da rede, com um Mempool cheio sugerindo tempos de confirmação mais longos. Como estrutura dinâmica, transações podem ser adicionadas ou removidas do Mempool com base em confirmações e necessidades de espaço.*"

No universo das criptomoedas, um dos conceitos mais cruciais a entender é o do Mempool, ou Pool de Memória. Esta estrutura de dados desempenha um papel crucial no processamento de transações e na garantia da integridade da blockchain.

O termo "Mempool" é uma combinação das palavras "memory" e "pool", e é essencialmente uma "área de espera" para todas as transações de criptomoedas não confirmadas. Cada nó em uma rede de blockchain mantém seu próprio Mempool, onde as transações pendentes são armazenadas até serem confirmadas e incluídas em um bloco por um minerador.

Quando um usuário inicia uma transação, ela é transmitida para todos os nós na rede. Cada nó verifica se a transação é válida (por exemplo, se o remetente tem fundos suficientes), e se for, a transação é adicionada ao Mempool. Lá, a transação aguarda até que um minerador a pegue e a inclua em um novo bloco.

Vamos entender isso com um exemplo. Suponha que Alice queira enviar 1 BTC para Bob. Alice cria a transação e a transmite para a rede Bitcoin. Cada nó recebe a transação, verifica sua validade e, se for válida, adiciona-a ao seu Mempool. Neste ponto, a transação de Alice está na "área de espera", não confirmada.

Agora, os mineradores entram em ação. Os mineradores pegam transações do Mempool para incluí-las em novos blocos. Ao escolher quais transações incluir, os mineradores normalmente priorizam transações com taxas mais altas, já que as taxas representam um incentivo para o minerador. Suponha que um minerador pegue a transação de Alice do Mempool, a inclua em um novo bloco e adicione esse bloco à blockchain. Agora a transação de Alice é confirmada e é removida do Mempool.

Além de ser uma "área de espera" para transações não confirmadas, o Mempool também serve como um indicador útil do congestionamento da rede. Se há muitas transações aguardando no Mempool e não há mineradores suficientes para confirmá-las, isso pode levar a tempos de confirmação mais longos e taxas mais altas. Isso é porque os usuários podem optar por pagar taxas mais altas para incentivar os mineradores a priorizar suas transações. Assim, um Mempool cheio pode indicar que a rede está congestionada.

Também é importante notar que cada nó na rede tem seu próprio Mempool e pode ter regras diferentes para aceitar transações. Isso significa que uma transação pode ser aceita no Mempool de um nó, mas rejeitada por outro. Além disso, se um nó sai da rede e depois se reconecta, seu Mempool pode ser diferente dos Mempools de outros nós.

Isso ocorre porque o Mempool de um nó reflete suas transações não confirmadas e pode ser influenciado por fatores como a latência da rede e a taxa de transmissão de transações. No entanto, a sincronização entre os nós é mantida por meio do consenso da blockchain, de modo que, eventualmente, todos os nós alcançam um estado de consenso sobre as transações confirmadas.

É importante observar que o Mempool é uma estrutura de dados temporária e dinâmica. As transações podem entrar e sair do Mempool à medida que são adicionadas e confirmadas nos blocos da blockchain. Portanto, as transações que permanecem no Mempool por um longo tempo sem serem confirmadas podem ser removidas pelo nó para liberar espaço para novas transações.