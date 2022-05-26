
##### docker volume
***


|Comando|Descrição|
|:--|:--|
|docker volume --help| Mostrar ajuda dos comandos do volume|
|docker volume ls | Mostrar os volumes|
|docker volume create \<volume\> | Criar o volume|
|docker volume inspect \<volume\>| Mostrar informações do volume|
|docker volume rm \<volume\>|Remover o volume|
|docker volume prune| Remover todos os volumes não usados|

***
**Observações:** 

1. Quando o diretório já existe usar  o type=bind e caso queira readonly adicionar ro.
**Exemplo:** `docker container run -ti --mount type=bind,src=d:\workspace\docker\bind,dst=/giropops,ro debian`

2. Quando precisamos adicionar o volume no container usar  o type=volume e passar no source o nome do volume.
**Exemplo:** `docker container run -ti --mount type=volume,src=giropops,dst=/giropops,ro debian`

