
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

**Modificadores de acesso**
*Public* - permite acesso a qualquer código externo a classe.
*Protected* - permite acesso às classes filhas e no mesmo pacote, mas proíbe a qualquer outro acesso externo.
*Default* - não escreve nada. No mesmo pacote ou dentro de mim para poder acessar.
*Private* - proíbe qualquer acesso externo à própria classe, inclusive das classes filhas.

| |public|protect|"default"|private|
|:--:|:--:|:--:|:--:|:--:|
|Classes e Interface|ok||ok||
|membros|ok|ok|ok|ok|
|classes internas|ok|ok|ok|ok|

***
**Assinatura**

-   `final` - em caso de herança, o método não pode ser sobrescrito nas classes filhas;
-   `abstract` - obriga as classes filhas a implementarem o método. O método abstrato **não** pode ter corpo definido;
-   `static` - método, atributo pertence à classe em que foi declarada, não a uma instância dela;
-   `synchronized` - _lock_ da instância;
-   `native` - Permite a implementação do método em código nativo (_JNI_);
-   `strictfp` - Ativa o modo de portabilidade matemática para contas de ponto flutuante.
-   `throws <EXCEPTIONS>` - após a lista de parâmetros, podemos indicar quantas exceptions quisermos para o `throws`.


