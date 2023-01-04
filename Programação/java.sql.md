***
-   Para acessar o banco de dados, precisamos de um **_driver_**
    -   Um _driver_ nada mais é do que uma biblioteca (JAR)
-   **JDBC** significa _Java DataBase Conectivity_
    -   JDBC define uma camada de abstração entre a sua aplicação e o _driver_ do banco de dados
    -   Essa camada possui, na sua grande maioria, interfaces que o _driver_ implementa
-   Para abrir uma conexão, devemos usar o método `getConnection`, da classe `DriverManager`
    -   O método `getConnection` recebe uma string de conexão JDBC, que define a URL, usuário, senha, etc
-   Para simplificar e encapsular a criação da conexão, devemos usar uma classe `ConnectionFactory`
    -   A classe `ConnectionFactory` segue o padrão de criação _Factory Method_
    -   O _Factory Method_ encapsula a criação de um objeto
-   Para executar um comando SQL, podemos usar a interface `java.sql.Statement`
    -   O método `execute` envia o comando para o banco de dados
    -   Dependendo do comando SQL, podemos recuperar a chave primária ou os registros selecionados
-   Ao executar SQL como `Statement`, temos um risco de segurança, chamado de **_SQL Injection_**
    -   _SQL Injection_ nada mais é do que passar um novo comando SQL como parâmetro
-   Para evitar _SQL Injection_, devemos usar a interface `PreparedStatement`
    -   Diferentemente do `Statement`, o `PreparedStatement` trata (_sanitiza_) cada parâmetro do comando SQL
-   O banco de dados oferece um recurso chamado de **transação**, para juntar várias alterações como unidade de trabalho
    -   Se uma alteração falha, nenhuma alteração é aplicada (é feito um _rollback_ da transação)
    -   Todas as alterações precisam funcionar para serem aceitas (é feito um `commit`)
-   `commit` e `rollback` são operações clássicas de transações
-   Para garantir o fechamento dos recursos, existe no Java uma cláusula _try-with-resources_
    -   O recurso em questão deve usar a interface `Autoclosable`
-   É boa prática usar um **_pool_ de conexões**
-   Um _pool_ de conexões administra/controla a quantidade de conexões abertas
    -   Normalmente tem um mínimo e máximo de conexões
-   Como existe uma interface que representa a conexão (`java.sql.Connection`), também existe uma interface que representa o _pool_ de conexões (`javax.sql.DataSource`)
-   **C3PO** é uma implementação Java de um _pool_ de conexão
-   Para cada tabela de domínio, temos uma classe de domínio
    -   Por exemplo, a tabela `produtos` tem uma classe `Produto` associada
    -   Objetos dessa classe representa um registro na tabela
-   Para acessar a tabela, usaremos um padrão chamado **_Data Access Object_** (**DAO**)
    -   Para cada classe de domínio, existe um DAO. Por exemplo, a classe `Produto` possui um `ProdutoDao`
    -   Todos os métodos JDBC relacionados com o produto devem estar encapsulados no `ProdutoDao`

### SITES
***
[Connection Strings](https://www.connectionstrings.com/)
