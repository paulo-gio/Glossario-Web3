# Gás (Gas)

>"*A Ethereum utiliza o mecanismo de 'gás' para quantificar o esforço computacional necessário para executar transações e contratos inteligentes na rede. Os usuários pagam taxas de gás em Ether (ETH) para garantir a execução de suas operações. Com o upgrade de Londres, a forma como as taxas são calculadas mudou, dando aos usuários mais controle sobre o valor que estão dispostos a pagar. O gás protege a rede contra abusos e incentiva os validadores a incluir transações em blocos através de taxas de prioridade.*"

Ethereum, uma plataforma líder em contratos inteligentes e que abriga a segunda maior criptomoeda em termos de capitalização de mercado, utiliza um mecanismo único e inovador conhecido como 'Gás'. Esse mecanismo desempenha um papel fundamental na execução de transações e operações na rede Ethereum, sendo uma unidade de medida que quantifica o esforço computacional necessário.

Assim como um veículo precisa de combustível para se movimentar, a rede Ethereum necessita de gás para funcionar. Cada transação ou contrato inteligente executado na Ethereum consome uma quantidade determinada de recursos computacionais. Portanto, para garantir a execução dessas operações, é necessário o pagamento de uma taxa denominada de gás.

As taxas de gás são pagas na moeda nativa da Ethereum, o Ether (ETH). Para tornar essas taxas mais compreensíveis e manejáveis, os preços do gás são expressos em 'gwei', uma denominação menor do ETH. Cada gwei equivale a 0.000000001 ETH (10-9 ETH). Isso significa que, ao invés de dizer que o gás para uma transação custa 0.000000001 ETH, é mais prático afirmar que custa 1 gwei.

Originalmente, a Ethereum operava com blocos de tamanho fixo. Em momentos de alta demanda na rede, esses blocos trabalhavam a plena capacidade, resultando muitas vezes numa experiência ruim para o usuário. O upgrade de Londres, implementado em agosto de 2021, solucionou essa questão ao introduzir blocos de tamanho variável na Ethereum.

Cada bloco tem um tamanho alvo de 15 milhões de gás. Porém, o tamanho real do bloco pode aumentar ou diminuir de acordo com a demanda na rede, até um limite de 30 milhões de gás, ou seja, o dobro do tamanho alvo.

Após o upgrade de Londres houve também uma mudança significativa na forma como as taxas de transação na rede Ethereum são calculadas. Antes deste upgrade, as taxas eram calculadas simplesmente multiplicando a quantidade de gás usada pela taxa de gás por unidade. Após o upgrade, a taxa total passou a ser o produto das unidades de gás usadas e a soma da taxa base e da taxa de prioridade.

A taxa base é um valor determinado pelo protocolo da Ethereum, enquanto a taxa de prioridade é um valor definido pelo usuário como uma espécie de gorjeta para o validador. Isso confere aos usuários mais controle sobre o quanto estão dispostos a pagar para ter suas transações processadas.

A taxa base é determinada comparando o tamanho do último bloco (a quantidade de gás usada para todas as transações nele incluídas) com o tamanho alvo do bloco. Se o tamanho alvo for excedido, a taxa base aumentará em um máximo de 12,5% por bloco, tornando economicamente inviável manter blocos constantemente cheios.

Já a taxa de prioridade é um valor adicional que pode ser estabelecido pelo usuário como uma "gorjeta" para incentivar os validadores a priorizarem sua transação. Sem essa taxa de prioridade, os validadores poderiam considerar economicamente mais viável validar blocos vazios, já que receberiam a mesma recompensa do bloco, mas com menos esforço computacional. As taxas de prioridade, portanto, atuam como um estímulo para os validadores incluírem transações nos blocos.

Ao realizar uma transação na rede Ethereum, os usuários podem estipular um limite máximo de gás que estão dispostos a pagar. Este limite é conhecido como 'limite de gás'. Se uma transação requerer mais gás do que o especificado no limite, a transação será interrompida e falhará. No entanto, todo o gás utilizado até o ponto de falha será consumido, representando um custo para o usuário mesmo sem a conclusão bem-sucedida da transação. Por outro lado, se a transação consumir menos gás do que o limite, o excesso será reembolsado ao usuário.

Os validadores, que são responsáveis por confirmar e registrar as transações na rede Ethereum, têm a liberdade de escolher quais transações incluir em um bloco. Em geral, eles preferem transações com taxas de gás mais altas, pois isso aumenta sua recompensa. Durante períodos de alta demanda, as taxas de gás podem aumentar significativamente, pois os usuários competem para que suas transações sejam incluídas nos blocos.

Com a introdução da taxa base e da taxa de prioridade pelo upgrade de Londres, os usuários ganharam mais flexibilidade na definição do custo de suas transações. Eles podem escolher pagar uma taxa de prioridade mais alta para incentivar os validadores a incluir sua transação em um bloco mais rapidamente. É importante entender que o gás na Ethereum não só garante a execução justa das transações e contratos inteligentes, mas também protege a rede contra abuso, limitando a quantidade de trabalho que cada transação pode exigir dos validadores.