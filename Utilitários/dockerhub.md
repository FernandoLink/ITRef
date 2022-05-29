
###### dockerhub
***
Plataforma de compartilhamento e gerenciamento de dockerfiles.

|Comando|Descrição|
|:--|:--|
|docker login| Logar no registry|
|docker push \<user docker hub\>\/\<reporsitory\>\:\<tag\>| Subir imagem no registry|
|docker pull \<user docker hub\>\/\<reporsitory\>\:\<tag\> | Baixar imagem no registry|
|docker logout| Deslogar do dockerhub|

**Obs.:** 

*Registry* - termo utilizado para repositório de imagens, como o dockerhub.

*.dockerignore* - serve para colocar os arquivos que deseja não pertender ao registry.
Deve estar no mesmo nível do Dockerfile.

**Exemplo: .dockerignore**
```
# comment
*/temp*
*/*/temp*
temp?
```


##### SITES
***
[Docker Hub](https://hub.docker.com/)

