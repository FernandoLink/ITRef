
##### Docker
***
**Docker** é um conjunto de produtos de plataforma como serviço que usam virtualização de nível de sistema operacional para entregar software em pacotes chamados contêineres.
Os contêineres são isolados uns dos outros e agrupam seus próprios softwares, bibliotecas e arquivos de configuração. 
Eles podem se comunicar uns com os outros por meio de canais bem definidos.
Todos os contêineres são executados por um único kernel do sistema operacional e, portanto, usam menos recursos do que as máquinas virtuais.
Um container tem várias camadas mas somente na última camada é read/write, as outras camadas são somente read.
Caso precise alterar as outras camadas, que não a última, o docker cria uma cópia identica e aí sim consegue alterar.

**Cgroups** (abreviação de "control groups") são usados ​​para limitar e controlar o uso de recursos do sistema por um conjunto de processos. Por exemplo, um cgroup pode ser configurado para limitar o uso de memória de um conjunto de processos para um determinado valor. Isso ajuda a evitar que um único processo consuma toda a memória disponível e prejudique o funcionamento do sistema.

**Namespaces** são usados ​​para criar um ambiente isolado para um conjunto de processos, de modo que esses processos vejam um conjunto diferente de recursos do sistema do que os processos fora do namespace. Por exemplo, um namespace de rede pode ser criado para um conjunto de processos, permitindo que eles vejam apenas uma parte da rede do sistema, enquanto outros processos não têm acesso a essa parte da rede.

***
`docker run hello-world`

***
**Isolamentos**
*PID* - provê isolamento dos processos rodando dentro do container.
*NET* - provê isolamento das interfaces de rede.
*IPC* - provê isolamento da comunicação entre processos e memória compartilhada.
*MNT* - provê isolamento do sistema de arquivos / pontos de montagem
*UTS* - provê isolamento do kernel. Age como se o container fosse um outro host.

***
|Comando|Descrição|
|:--|:--|
|docker version ou --version|Verificar a versão do docker|
|docker --help| Mostra ajuda dos comandos do docker|
| docker info| Mostra informações do docker|
|docker login| Login no docker|
|docker logout| Logout no docker|

***
* [[docker container]]
* [[docker image]]
* [[docker volume]]
* [[docker commit]]
* [[docker swarm]]
* [[docker node]]
* [[dockerfile]]
* [[dockerhub]]
* [[docker service]]

***

##### SITES
***
[Docker](https://www.docker.com/)
[Documentação](https://docs.docker.com/)
[Docker Hub](https://hub.docker.com/)












