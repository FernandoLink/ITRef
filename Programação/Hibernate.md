***
**Ciclo de Vida**

![[Pasted image 20230105185552.png]]


Relacionamentos _to many_ já são _lazy_, você não precisa colocar, agora, os _to one_, são _eager_ por padrão.

`@ManyToOne(fetch = FetchType.LAZY)`

