
##### docker swarm
***


|Comando|Descrição|
|:--|:--|
|docker swarm --help| Mostrar ajuda dos comandos do swarm|
|docker swarm init| Inicializar o swarm|
|docker swarm join-token --help| Mostrar ajuda do join-token|
|docker swarm join-token manager| Mostra o token do manager|
|docker swarm join-token worker|Mostra o token do worker|
|docker swarm join-token --rotate \< manager ou worker\>| Rotacionar os nodes|

***
**Worker** - principal função ter containers em execução.
**Manager** - esta toda a administração do cluster.

*Obs.:* Para ter resiliência precisamos de 51% dos meus managers funcionando.
Sempre temos que ter mais que 50% dos clusters managers em pé, para não perder o meu cluster.
