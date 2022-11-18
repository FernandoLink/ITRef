
##### Métodos
***

**Procedimento**
```
static void soma(int a, int b) {
    int s = a + b;
    System.out.println("A soma é " + s);
}
```

**Função**
```
static int soma(int a, int b) {
    int s = a + b;
    return s;
}
```

***

**Obs.:** 
*Static* - serve para dizer que o método pertence à classe em que foi declarada, não a uma instância dela.

***
**Modificadores de acesso**
*Public* - permite acesso a qualquer código externo a classe.
*Protected* - permite acesso às classes filhas, mas proíbe a qualquer outro acesso externo.
*Private* - proíbe qualquer acesso externo à própria classe, inclusive das classes filhas.




