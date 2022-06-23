
##### docker container
***


|Comando|Descrição|
|:--|:--|
|docker container --help| Mostra ajuda dos comandos do container|
|docker container \<commando\> --help| Mostrar ajuda do comando|
|ctlr+p+q| Sair do container sem destruí-lo|
|docker container ls| Listar os containers ativos|
|docker container ls -a| Listar os containers ativos/inativos|
|docker container run -ti \<container\>| Docker executa o container, -ti terminal e interatividade|
|docker container run -d \<container\>| Docker executa o container, -d deamon não rodar em primeiro plano|
|docker container run -d -m 128M \<container\>| Docker executa o container limitando memória a 128M|
|docker container attach \<container ID ou names\>| Voltar para o container|
|docker container exec -ti \<container ID\> \<command\>| Executar comando em containers deamon|
|docker container stop \<container ID\>| Parar a execução do container|
|docker container start \<container ID\>|Startar o container|
|docker container restart \<container ID\>|Restartar o container|
|docker container inspect \<container ID\>|Mostrar informações detalhadas do container|
|docker container pause \<container ID\>|Pausar o container|
|docker container unpause \<container ID\>|Despausar o container|
|docker container logs -f \<container ID\>|Ver os logs de um container|
|docker container rm -f \<container ID\>|Remover container -f force |
|docker container stats \<container ID\>|Mostrar estatísticas CPU, MEM e NET|
|docker container top \<container ID\>|Mostrar os processos rodando no container|
|docker container update \<param\> \<container ID\>|Atualiza configuração do container|
|docker container prune| Remove todos os containers parados|
|docker container create --name \<nome\> | Criar container sem inicializá-lo|


