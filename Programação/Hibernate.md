***
**Ciclo de Vida**

![[Pasted image 20230105185552.png]]


Relacionamentos _to many_ já são _lazy_, você não precisa colocar, agora, os _to one_, são _eager_ por padrão.

`@ManyToOne(fetch = FetchType.LAZY)`

-   A utilizar as anotações `@Embeddable` e `@Embedded` para organizar o código de uma entidade;
-   A realizar herança entre entidades com as estratégias `SINGLE_TABLE` e `JOINED`;
-   Como mapear uma chave composta com a anotação `@EmbeddedId`.