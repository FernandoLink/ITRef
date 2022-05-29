
##### Docker
***
**Docker** é um conjunto de produtos de plataforma como serviço que usam virtualização de nível de sistema operacional para entregar software em pacotes chamados contêineres.
Os contêineres são isolados uns dos outros e agrupam seus próprios softwares, bibliotecas e arquivos de configuração. 
Eles podem se comunicar uns com os outros por meio de canais bem definidos.
Todos os contêineres são executados por um único kernel do sistema operacional e, portanto, usam menos recursos do que as máquinas virtuais.
Um container tem várias camadas mas somente na última camada é read/write, as outras camadas são somente read.
Caso precise alterar as outras camadas, que não a última, o docker cria uma cópia identica e aí sim consegue alterar.

***
|Comando|Descrição|
|:--|:--|
|docker version ou --version|Verificar a versão do docker|
|docker --help| Mostra ajuda dos comandos do docker|

***
* [[docker container]]
* [[docker image]]
* [[docker volume]]
* [[docker commit]]
* [[dockerfile]]
* [[dockerhub]]

***

##### SITES
***
[Docker](https://www.docker.com/)
[Documentação](https://docs.docker.com/)
[Docker Hub](https://hub.docker.com/)












