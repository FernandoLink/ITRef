***
-   Apache Tomcat ou apenas Tomcat é um servidor web em Java
-   Tomcat _entende_ o protocolo HTTP e roda por padrão no `http://localhost:8080`
-   O projeto Java faz parte da URL, no nosso caso: `http://localhost:8080/gerenciador`
-   Uma aplicação web Java pode ter páginas HTML
-   Uma servlet é um objeto Java que podemos chamar a partir de uma requisição HTTP
-   Para mapear a URL para uma servlet usamos a anotação `@WebServlet`
-   Uma servlet deve estender a classe `HttpServlet` e sobrescrever um determinado método (por exemplo `service`)


***
[JSTL](https://tomcat.apache.org/taglibs/standard/) - JSP Standard Tag Library

* **core** - controle de fluxo
`<%@ taglib uri="http://java.sun.com/jsp/jstl/core" prefix="c"%>`
* **fmt** - formatação / i18n (internacionalização)
`<%@ taglib uri="http://java.sun.com/jsp/jstl/fmt" prefix="fmt"%>`
* **sql** - executar SQL
* **xml** - gerar XML
