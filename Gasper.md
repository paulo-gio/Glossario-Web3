# Gasper

>"*O Gasper é um protocolo de consenso da Ethereum 2.0 que combina os mecanismos Casper FFG e LMD GHOST. Ele utiliza a Prova de Participação (PoS) e é responsável por definir incentivos e penalidades para os validadores. Os validadores participam do protocolo validando dados e são recompensados com Ether. A finalidade é uma propriedade importante do Gasper, garantindo que certos blocos não possam ser revertidos, a menos que ocorra uma falha crítica de consenso.*"

Gasper, um protocolo de consenso na cadeia Beacon da Ethereum 2.0 que usa a Prova de Participação (PoS) para adicionar novos blocos à cadeia, desempenha um papel crucial ao definir incentivos e penalidades para os validadores. Sendo uma combinação de dois mecanismos, Casper, o Gadget de Finalidade Amigável (Casper the Friendly Finality Gadget, ou Casper FFG) e LMD GHOST (Latest Message-Driven Greedy Heaviest Observed SubTree), o Gasper é responsável por determinar quais blocos devem ser aceitos ou rejeitados, e qual fork - ou bifurcação - da blockchain deve ser usado.

Casper FFG é um mecanismo que opera sobre uma blockchain existente e marca certos blocos como finalizados. A finalização dos blocos fornece aos usuários da blockchain a certeza de que esses blocos fazem parte da cadeia principal e não serão revertidos. O LMD GHOST, por outro lado, é uma regra de escolha de fork que ajuda a escolher entre muitas cadeias de forks. Ele auxilia na escolha do fork com o maior peso acumulado de votos do validador.

Os validadores são entidades que participam do protocolo para fins de validação de dados. Eles são responsáveis por propor e atestar blocos, ou seja, votar que um certo bloco é válido. Para se tornarem validadores, eles devem colocar em stake - ou participar com - uma certa quantidade de Ether na cadeia Ethereum. Os validadores são conectados através de uma rede ponto a ponto (p2p), onde os blocos são tipos especiais de mensagens que podem ser transmitidas entre validadores.

A comunicação entre validadores é realizada através de mensagens. Quando um validador honesto transmite uma mensagem, assume-se que ela é enviada para todos os validadores na rede. No entanto, um validador malicioso pode optar por não enviar quaisquer mensagens para sabotar o sistema ou censurar alguma informação que deseje usar em seu próprio benefício.

Um aspecto importante de Gasper é a finalidade. A finalidade é uma propriedade de certos blocos que significa que eles não podem ser revertidos a menos que tenha ocorrido uma falha crítica de consenso e um invasor tenha destruído pelo menos 1/3 do total do Ether em stake. Para que um bloco seja finalizado, ele deve passar por um procedimento de upgrade de duas etapas, onde dois terços do total de Ether em stake deve ter votado a favor da inclusão desse bloco na cadeia canônica.

Os validadores são recompensados por propor e validar blocos honestamente. Ether é recompensado e adicionado à sua participação. No entanto, os validadores que estão ausentes e não agem quando são convocados, perdem essas recompensas e, às vezes, perdem uma pequena parte de sua participação existente.

Além de segurança, o Gasper também fornece "viabilidade plausível". Essa é a condição de que, desde que dois terços do total de Ether em stake esteja votando honestamente e seguindo o protocolo, a cadeia será capaz de finalizar, independentemente de qualquer outra atividade. No Gasper, existe um mecanismo adicional de defesa contra uma falha de viabilidade, conhecido como "vazamento de inatividade". Esse mecanismo é ativado quando a cadeia falha em finalizar por mais de quatro épocas (epochs).

Finalmente, o Gasper utiliza o algoritmo de escolha de fork LMD GHOST para decidir entre diferentes cadeias de blocos. Basicamente, cada validador tem um "última mensagem" que eles enviaram, e esta mensagem é considerada como um voto para uma determinada cadeia de blocos. LMD GHOST opera analisando essas últimas mensagens e optando pela cadeia que tem a maioria dos votos ponderados dos validadores.

Vamos considerar um exemplo simples. Suponha que temos dois forks, Fork A e Fork B. Se o número total de ETH em stake dos validadores cuja última mensagem aponta para o Fork A é maior do que o total em stake dos validadores cuja última mensagem aponta para o Fork B, então o algoritmo escolherá o Fork A como a cadeia principal.

Deste modo, LMD GHOST proporciona um meio robusto de selecionar entre diferentes forks. Ao considerar as últimas mensagens dos validadores, leva em conta a atividade mais recente na rede, o que ajuda a garantir que a escolha do fork reflete o estado atual do consenso entre os validadores.

Além disso, Gasper utiliza uma abordagem de finalidade híbrida, o que significa que além de usar a Prova de Participação para adicionar novos blocos à cadeia, também usa a finalidade de Casper FFG para garantir que certos blocos não possam ser revertidos.

A combinação desses elementos - Casper FFG, LMD GHOST, e o sistema de recompensas e penalidades - proporciona uma segurança robusta e eficiente para a Ethereum 2.0 e foi um passo crucial na transição da Ethereum do modelo de Prova de Trabalho para o modelo atual de Prova de Participação.