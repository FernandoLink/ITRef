***
-   **Entity**: Uma entidade é uma classe que representa algo que possui uma identidade única e que precisa ser persistido em algum lugar. Em geral, entidades são objetos que possuem um identificador único (ID) e propriedades que definem suas características. Por exemplo, em um sistema de vendas, uma entidade poderia ser um cliente, um pedido ou um produto.
    
-   **Value Object**: Um objeto de valor é uma classe que representa um valor sem identidade própria. Em outras palavras, seu valor é determinado exclusivamente pelas propriedades que possui. Por exemplo, em um sistema de vendas, um objeto de valor poderia ser um preço, uma data ou um endereço.
    
-   **Repository**: Um repositório é uma classe responsável por persistir e recuperar entidades do banco de dados ou de outra fonte de dados. Ele abstrai o acesso ao armazenamento e oferece uma interface simples e padronizada para o restante da aplicação.
    
-   **Factory**: Uma fábrica é uma classe responsável por criar objetos complexos, geralmente agregados de objetos, com várias dependências. Ela encapsula a lógica de criação desses objetos e permite que o código cliente se concentre apenas na utilização do objeto criado.
    
-   **Service**: Um serviço é uma classe que representa uma ação que pode ser executada na aplicação. Ele encapsula a lógica de negócio e pode ou não interagir com entidades, objetos de valor, repositórios ou fábricas. Por exemplo, em um sistema de vendas, um serviço poderia ser responsável por calcular o valor total de um pedido, validar uma transação de pagamento ou enviar um e-mail de confirmação de compra.