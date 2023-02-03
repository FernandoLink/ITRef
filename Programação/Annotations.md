***
**java.lang.annotation**

No Java, existem 5 meta anotações, são elas:

-   **@Retention** - especifica como a anotação deve ser considerada pelo Java. Seus possíveis valores são:
    
    -   **RetentionPolicy.SOURCE** – A anotação é considerada apenas a nível de código fonte e ignorada pelo compilador.
    -   **RetentionPolicy.CLASS (valor padrão)** – A anotação é levada em consideração pelo compilador em tempo de compilação, mas ignorada pela JVM em tempo de execução.
    -   **RetentionPolicy.RUNTIME** – A anotação será considerada pela JVM em tempo de execução.
-   **@Documented** - Indica se a anotação deve ser documentada no Javadoc juntos aos elementos onde for utilizada.
    
-   **@Target** - Indica onde a anotação pode ser utilizada no código Java. Seus possíveis valores são:
    
    -   **ElementType.ANNOTATION_TYPE** - pode ser aplicada numa anotação.
    -   **ElementType.CONSTRUCTOR** - pode ser aplicada num construtor.
    -   **ElementType.FIELD** - pode ser aplicada num atributo.
    -   **ElementType.LOCAL_VARIABLE** - pode ser aplicada numa variável local.
    -   **ElementType.METHOD** - pode ser aplicado num método.
    -   **ElementType.PACKAGE** - pode ser aplicada numa declaração de pacote.
    -   **ElementType.PARAMETER** - pode ser aplicada num parâmetro de método.
    -   **ElementType.TYPE** - pode ser aplicada na declaração de uma classe, interface (incluindo anotações) ou enum.
-   **@Inherited** - indica que a anotação será herdada por classes filhas quando usada numa super classe. Essa herança não ocorre por padrão! Além disso, anotações "herdáveis" só podem ser aplicadas em classes.
    
-   **@Repeatable** - introduzida a partir do Java 8, indica que a anotação pode ser aplicada mais de uma vez no mesmo lugar.



