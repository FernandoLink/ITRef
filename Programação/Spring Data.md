***

-   A integrar o módulo Spring Data JPA
    -   Configuramos as dependências no `pom.xml`
    -   Configuramos os dados da conexão pelo `application.properties`
-   Que, para usar o **Spring Data JPA**, basta criar uma interface e:
    -   Usar a anotação `@Repository`
    -   Estender uma interface do Spring como `JpaRepository`
-   Que um repositório padrão do Spring já tem vários métodos implementados. como `findAll`, `save`, `delete` ou `findById`
-   Que, para receber uma instância do repositório, usamos a **injeção de dependências**
