
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

3. Criar temporário (tmpfs) e só funciona no linux.
**Exemplo:** `docker container run -ti --tmpfs=/app debian`
***
*tmpfs* é um tipo de sistema de arquivos que é armazenado em RAM e não em disco. Isso significa que os arquivos e pastas criados em um tmpfs são armazenados na memória RAM do host, ao invés de em um disco.