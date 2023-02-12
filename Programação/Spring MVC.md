***

-   Para gerar o projeto usamos o Spring Initialzr: [https://start.spring.io/](https://start.spring.io/)
-   Usamos o Spring Boot para inicializar a aplicação e rodar o Tomcat
-   Spring Boot já tem o servlet container Tomcat embutido
-   Spring MVC segue o padrão arquitetural Model-View-Controller
-   O servlet do Spring MVC recebe as requisições e delega para controllers mais específicos
-   Como View, o Spring MVC usa Thymeleaf
-   O Thymeleaf é uma alternativa a tecnologia JSP, serve para gerar HTML dinamicamente
-   Thymeleaf tem a vantagem de usar atributos para definir a _expression language_
-   Para definir uma classe que responde uma requisição HTTP, usamos as anotações:
    -   `@Controller`, `@GetMapping` entre outras opções
-   Métodos que atendem requisições HTTP são chamados de *action*
-   Como usar um modelo nosso para a view
-   Como iterar com Thymeleaf e trabalhar com inputs e imagens
-   Como aplicar classes do Bootstrap e posicionar elementos de maneira responsiva