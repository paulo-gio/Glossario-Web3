# Trie Merkle Patricia, Trie de Compressão de Prefixo (Merkle Patricia Trie)

>"*A Trie Merkle Patricia combina as características das Tries Patricia e árvores Merkle para fornecer armazenamento eficiente e autenticação criptográfica de associações (chave, valor). Essa estrutura compacta e segura é amplamente utilizada em sistemas distribuídos e blockchain, como na Ethereum, para armazenar e autenticar diversos tipos de dados, desempenhando um papel fundamental na segurança e funcionalidade dessas plataformas.*"

A Trie Merkle Patricia é uma estrutura de dados que combina as características das Tries Patricia e árvores Merkle para fornecer um armazenamento eficiente e autenticação criptográfica de associações (chave, valor).

A Patricia Trie é uma forma otimizada de Trie, que armazena as chaves nos nós da árvore, mas utiliza representação binária para comprimir e otimizar o espaço de armazenamento. O nome Patricia não é um acrônimo, mas uma abreviação do termo "Practical Algorithm To Retrieve Information Coded In Alphanumeric".

As árvores Merkle, por outro lado, são estruturas de dados que fornecem autenticação e integridade criptográfica, sendo amplamente utilizadas em sistemas distribuídos e blockchain. Em uma árvore Merkle, cada nó contém o hash criptográfico de seus filhos, e esse hash é usado para verificar a integridade dos dados.

A Trie Merkle Patricia combina essas duas estruturas de dados para fornecer um sistema eficiente e seguro de armazenamento de informações. Em vez de armazenar cada palavra completa na Trie, a Trie Merkle Patricia agrupa vários caracteres em blocos. Cada bloco é associado a uma função hash criptográfica, geralmente a função Keccak-256.

A autenticação criptográfica na Trie Merkle Patricia é alcançada por meio da inclusão dos hashes dos blocos em cada nó interno da árvore. Isso permite que qualquer modificação nos dados armazenados resulte em uma alteração nos hashes dos nós afetados e, consequentemente, em toda a estrutura.

A inserção, pesquisa e exclusão de associações (chave, valor) em uma Trie Merkle Patricia são eficientes, pois a complexidade do tempo de operação é proporcional ao comprimento da chave, e não ao número total de chaves. Isso se deve à estrutura compacta da Trie Merkle Patricia e à verificação dos hashes, o que permite uma busca rápida pelos dados desejados.

A estrutura compacta da Trie Merkle Patricia reduz o espaço de armazenamento necessário, combinando nós consecutivos que têm apenas um filho. Isso resulta em um número menor de nós na árvore, e portanto, em menos comparações e acessos necessários durante as operações de inserção, pesquisa e exclusão.

Além disso, a verificação dos hashes é fundamental para a autenticação e integridade dos dados armazenados na Trie Merkle Patricia. Os hashes são usados para verificar se os nós da árvore não foram modificados, o que garante a consistência dos dados.

Graças a essas características, as operações em uma Trie Merkle Patricia têm uma complexidade de tempo proporcional ao comprimento da chave, o que significa que o tempo de execução aumenta de forma gradual e previsível à medida que o comprimento da chave aumenta. Isso torna a Trie Merkle Patricia uma estrutura de dados eficiente para lidar com grandes volumes de dados e realizar operações de busca e manipulação de associações (chave, valor) de forma rápida e escalável.

A Trie Merkle Patricia também oferece suporte a buscas eficientes por prefixo. Ao fornecer um prefixo, a estrutura percorre a Trie de forma apropriada, aproveitando a estrutura da árvore para localizar as associações relevantes.

Na camada de execução da Ethereum, são utilizadas as Tries Merkle Patricia para armazenar e autenticar diversos tipos de dados. Essas estruturas de dados combinam as propriedades das Tries Patricia, que são otimizadas para armazenar chaves de tamanho variável, com as propriedades das árvores Merkle, que fornecem autenticação criptográfica. Essas Tries desempenham um papel fundamental na segurança e na funcionalidade da plataforma Ethereum, permitindo o armazenamento eficiente, a recuperação de dados e a autenticação criptográfica dos diversos elementos relacionados a contas, contratos, transações e recibos na rede Ethereum.