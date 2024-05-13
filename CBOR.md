# CBOR, Concise Binary Object Representation (Representação Concisa de Objetos Binários) 

>"*O Concise Binary Object Representation (CBOR) é um formato de dados binários eficiente e compacto que codifica tipos de dados semelhantes aos usados pelo JSON, mas com suporte a tipos adicionais. Foi especificado pela IETF na RFC 7049 e é amplamente utilizado em comunicações na Internet das Coisas (IoT) e em redes ponto a ponto (p2p), como o IPFS. A principal diferença entre CBOR e JSON é que o CBOR é binário, o que o torna mais rápido e menor em tamanho.*"

O Concise Binary Object Representation (CBOR) é um formato de dados binários que codifica os tipos de dados utilizados pelo JSON e alguns outros tipos adicionais de maneira eficiente e compacta. Foi especificado pela primeira vez na RFC 7049 pela Internet Engineering Task Force (IETF) e é frequentemente usado em situações onde o tamanho e a velocidade são de grande importância, tais como comunicações na Internet das Coisas (IoT) ou redes ponto a ponto (p2p) como o InterPlanetary File System (IPFS) através do IPLD.

A principal diferença entre CBOR e JSON é que o primeiro é um formato binário, enquanto o segundo é um formato de texto. Isso permite que o CBOR seja mais eficiente em termos de tamanho e velocidade, uma vez que os dados binários podem ser processados mais rapidamente e ocupam menos espaço do que os dados de texto. Além disso, ao contrário do JSON, o CBOR suporta diretamente mais tipos de dados, incluindo números de precisão arbitrária, binários brutos, e tipos de dados mais complexos como mapeamentos e listas ordenadas.

Uma característica chave do CBOR é sua extensibilidade. Novos tipos de dados podem ser adicionados ao CBOR sem quebrar a compatibilidade com versões anteriores. Isso é feito usando um esquema de codificação de tag, onde cada tipo de dados tem uma tag numérica única. Se um decodificador CBOR encontra uma tag que não entende, ele pode simplesmente ignorá-la e continuar decodificando o resto dos dados.

O CBOR é compatível com a maioria das linguagens de programação modernas, com bibliotecas disponíveis para C, C++, Java, JavaScript, Python, Go, Rust e muitas outras. As bibliotecas CBOR geralmente fornecem uma API de alto nível que permite aos desenvolvedores trabalhar com dados CBOR como se fossem estruturas de dados nativas da linguagem de programação que estão usando.

Uma aplicação comum do CBOR é na Internet das Coisas (IoT), onde os dispositivos frequentemente precisam enviar e receber dados pequenos e eficientes. Como o CBOR é compacto, eficiente e fácil de analisar e gerar, é uma escolha natural para esses tipos de aplicações. Por exemplo, um dispositivo de IoT pode usar CBOR para enviar dados de sensor para um servidor em um formato que seja fácil de interpretar e processar.

Além disso, o CBOR é usado no IPLD (InterPlanetary Linked Data), uma parte do InterPlanetary File System (IPFS). O IPLD usa CBOR para codificar dados estruturados que podem ser vinculados entre si para criar uma web de dados descentralizada. A escolha do CBOR para esta aplicação deve-se à sua eficiência, extensibilidade e capacidade de representar uma ampla variedade de tipos de dados.

Uma vantagem importante do CBOR sobre outros formatos binários, como o Protocol Buffers (protobuf) do Google, é que ele não requer um esquema predefinido. Em vez disso, ele codifica o tipo de dados diretamente nos dados, o que significa que os dados CBOR podem ser decodificados sem precisar conhecer o esquema com antecedência. Isso torna o CBOR mais flexível e fácil de usar em situações onde os esquemas de dados podem mudar com o tempo.

O CBOR também suporta a codificação de dados autodescritivos, que incluem informações sobre o tipo de dados que estão sendo codificados. Isso é útil em situações onde os dados podem ser interpretados de várias maneiras, como por exemplo quando números podem ser interpretados como inteiros ou ponto flutuante.

No entanto, como qualquer tecnologia, o CBOR não é perfeito e tem suas desvantagens. Por exemplo, como é um formato binário, não é fácil para os humanos lerem ou escreverem diretamente. Além disso, embora o CBOR seja geralmente mais eficiente do que o JSON, ainda pode ser menos eficiente do que outros formatos binários que requerem esquemas, como o Protocol Buffers.

