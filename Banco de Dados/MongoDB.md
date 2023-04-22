***
MongoDB é um projeto open source com distribuição gratuita para Linux, Mac e Windows. Ele está disponível em duas edições de servidor: Community e Enterprise.

A versão **[Community edition](https://www.mongodb.com/)** é a edição gratuita do MongoDB disponível para fins de avaliação e desenvolvimento. Com a versão **Community edition**, pode-se criar diversos bancos de dados e coleções, além de tudo, trabalhar com diversos documentos e realizar diversas análises dos dados.

Já a versão **[Enterprise edition](https://www.mongodb.com/products/mongodb-enterprise-advanced?tck=docs_server)** é a edição comercial do MongoDB. Ela inclui recursos adicionais não disponibilizados na versão gratuita, como recursos avançados de segurança, assistência especializada, ferramentas poderosas, entre outros.

Além das duas versões de servidores, o MongoDB também disponibiliza a sua versão hospedada na nuvem, o **[MongoDB Atlas](https://www.mongodb.com/atlas/database?tck=docs_server)**. Você pode experimentar o **Atlas** gratuitamente com um cluster de 512 MB disponibilizado pela MongoDB.
***
O *Sharding* é uma técnica para distribuir os dados em um cluster MongoDB em vários servidores, ou seja, em vários shards. Cada shard contém uma parte dos dados e todos os shards juntos compõem o conjunto completo de dados. O Sharding permite que você aumente a capacidade de armazenamento e o poder de processamento do seu banco de dados, tornando-o mais escalável e permitindo que você lide com grandes quantidades de dados.

O *Replica Set* é um conjunto de servidores que mantêm cópias idênticas dos dados do MongoDB. O Replica Set é uma solução de alta disponibilidade que oferece redundância de dados e tolerância a falhas. Se um dos servidores falhar, um dos outros servidores pode assumir o controle, garantindo que os dados permaneçam disponíveis e que o sistema continue funcionando. O Replica Set também permite que você execute operações de leitura em réplicas secundárias, reduzindo a carga no servidor primário e melhorando o desempenho geral do sistema.
***
**BSON** é uma abreviação de "*Binary JSON*" e é um formato de serialização binária usado pelo MongoDB para armazenar e transmitir dados. O BSON é semelhante ao formato JSON, mas é projetado para ser mais eficiente em termos de armazenamento e transmissão, especialmente quando se trata de dados binários e tipos de dados mais complexos.

O BSON é um formato de serialização binária porque converte os dados em uma sequência de bytes, que podem ser facilmente armazenados em disco ou transmitidos pela rede. Ele é usado pelo MongoDB como o formato padrão de armazenamento de documentos e é usado para transferir dados entre clientes e servidores MongoDB.

O BSON é uma extensão do formato JSON e suporta tipos de dados adicionais, como BinData (dados binários), Date (data e hora), ObjectId (ID exclusivo do MongoDB), Regular Expression (expressão regular), e outros tipos de dados específicos do MongoDB. O BSON é mais compacto que o JSON, o que torna a transmissão de dados mais rápida e consome menos recursos de armazenamento.
***
**Observações**
* Os nomes de banco de dados não podem conter o caractere nulo.
* Os nomes de banco de dados não pode estar vazios e devem ter menos de 64 caracteres.
* Os nomes das coleções devem começar com um sublinhado ou um caractere de letra.
* Ser uma string vazia.
* Documentos são análogos a databases relacionais.
* Coleções são análogas as tabelas em um database relacional.
* O tamanho máximo de um documento BSON é 16 megabytes.
***

[[Commands]]

***

##### SITES
***
[MongoDB](https://www.mongodb.com/)
[BSON Types](https://www.mongodb.com/docs/manual/reference/bson-types/)
[BSON Specification](https://bsonspec.org/)

