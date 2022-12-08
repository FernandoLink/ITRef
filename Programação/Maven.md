

##### Maven
***

O Apache Maven é uma ferramenta de gerenciamento e compreensão de projetos de software. 
Baseado no conceito de um modelo de objeto de projeto (POM), a Maven pode gerenciar a construção, relatórios e documentação de um projeto.


***Valores padrão para os arquivos de código fonte do projeto***
|Item|Default|
|:--:|:-:|
| código fonte| ${basedir}/src/main/java|
|recursos|${basedir}/src/main/resources|
|testes|${basedir}/src/test/java|
| recursos de testes| ${basedir}/src/test/resources|
|compilador byte code|${basedir}/target|
|distribuível JAR|${basedir}/target/classes|


* Cache local do Maven **.m2**

Goals:
* **clean** - limpa o projeto e remove todos os arquivos gerados pela compilação anterior.
* **validate** - valida se o pom.xml está correto.
* **compile** - MyApp.java -> MyApp.class.
* **test** - roda os testes unitários.
* **package** - MyApp.class -> MyApp.jar.
* **integration test** - roda os testes de integração.
* **verify** - verificar se o projeto é válido.
* **install** - copia MyApp.jar to .m2/groupId/MyApp.jar.
* **deploy** - copia MyApp.jar para repositório maven central.


##### SITES
***
[Maven Repository](https://mvnrepository.com/)
