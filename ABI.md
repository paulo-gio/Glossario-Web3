# ABI, Application Binary Interface (Interface Binária de Aplicativos)

>"*Uma Interface Binária de Aplicativos (ABI) é um conjunto de regras de baixo nível que especificam a interação entre módulos de programas binários, como um programa e uma biblioteca do sistema operacional. As ABIs lidam com a convenção de chamadas, representação de tipos de dados em nível binário, sequência de argumentos, gerenciamento de exceções, alocação de memória, layout de código binário, ligação de módulos e medidas de segurança. Essas interfaces são cruciais para garantir a correta interpretação e manipulação dos dados entre componentes do sistema.*"

Em ciência da computação, uma Interface Binária de Aplicativos (ABI) é um conjunto de regras que define a interação entre dois módulos de programas binários. Normalmente, um desses módulos é uma biblioteca ou uma parte do sistema operacional, e o outro é um programa em execução. A ABI estabelece como as funções ou rotinas computacionais são chamadas e como as estruturas de dados são transmitidas entre esses módulos.

Diferente das APIs, a ABI opera em um formato de baixo nível e dependente do hardware, sendo específica para um sistema operacional, plataforma de hardware ou arquitetura de processador particulares. Uma das principais características da ABI é a convenção de chamada, prescrevendo como as funções são convocadas e como os dados são passados para elas. Há várias convenções de chamada, como a convenção de chamada C, amplamente adotada em sistemas baseados em UNIX, e a convenção de chamada x86, usada em sistemas baseados em processadores Intel.

A ABI também é responsável pela representação de tipos de dados em nível binário, garantindo a interpretação correta dos dados pelos módulos que interagem entre si. Além disso, a ABI estabelece a sequência em que os argumentos são passados para as funções, a maneira como os valores de retorno são manuseados e como as exceções são gerenciadas.

Em termos de gestão de memória, a ABI é fundamental, especificando como a memória é alocada e desalocada, a manipulação de ponteiros e o alinhamento de dados na memória. Essa última é especialmente importante para garantir um acesso eficiente da CPU aos dados.

A ABI também é crucial no layout do código binário, determinando a organização do código e dos dados dentro do arquivo binário. Isso inclui a disposição dos segmentos de código e de dados, a localização e formatação das tabelas de símbolos e o formato dos registros de depuração.

As ABIs também definem os mecanismos de ligação entre diferentes módulos de software, estipulando como as referências a funções ou variáveis externas são resolvidas e como as bibliotecas dinâmicas são carregadas e vinculadas. No campo da segurança, a ABI pode especificar como as proteções de memória são aplicadas, como o endereço de espaço de layout randomizado (ASLR) é utilizado e como outras medidas de mitigação de explorações são implementadas.

Frequentemente, as ABIs são documentadas e padronizadas, facilitando o desenvolvimento de produtos compatíveis por diferentes fornecedores de software e hardware. Um exemplo é a ABI do sistema operacional Linux para a arquitetura de processador x86, documentada e mantida pelo projeto Linux e pela comunidade de desenvolvedores.

A compreensão da ABI é essencial no desenvolvimento de software de baixo nível e na engenharia de sistemas, já que a ABI é a "cola" que une os diferentes componentes do sistema e possibilita que eles operem de forma coesa.

Para ilustrar, imagine um desenvolvedor criando um aplicativo que precisa interagir com uma biblioteca de software. A biblioteca usa a convenção de chamada C, onde os argumentos são passados de maneira específica e o valor de retorno é passado por um registrador. Se o aplicativo não conhecer essa convenção, pode passar argumentos na ordem errada ou procurar o valor de retorno no lugar errado, resultando em falhas.

Da mesma forma, a ABI determinará como os dados são representados em nível binário. Se a biblioteca usa uma representação de ponto flutuante de precisão dupla de 64 bits para números reais, o aplicativo deve usar a mesma representação para que os números sejam interpretados corretamente.

A ABI também definirá o gerenciamento de exceções. Se uma função da biblioteca levanta uma exceção, o aplicativo precisa saber como essa exceção será passada para ele para que possa ser tratada corretamente. Portanto, a compreensão e a aderência à ABI são essenciais para o desenvolvimento de software de baixo nível.