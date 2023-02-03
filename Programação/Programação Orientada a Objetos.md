
##### Programação Orientada a Objetos (POO)
***

**O que é um objeto?**
Coisa material ou abstrata que pode ser percebida pelos sentidos e descrita por meio das suas *características*, *comportamentos* e *estado* atual.

**Todo objeto tem:**
* *Atributos* - Coisas que eu tenho(*características*).
* *Métodos* - Coisas que faço (*comportamentos*).
* *Estado* - Como eu estou agora (*estado*)?

**Observações:** 
- Todos os objetos vem de uma classe. 
* Instanciar é quando pego uma classe e gero um objeto.

**Portanto:**
*Classe* -  Define os atributos e métodos comuns que serão compartilhados por um objeto.
*Objeto* -  É a instância de uma classe.

***

**Vantagens da POO:**
* *Confiável* - O isolamento entre as partes gera software seguro. Ao alterar uma parte, nenhuma outra é afetada.
* *Oportuno* - Ao dividir tudo em partes, várias delas podem ser desenvolvidas em paralelo.
* *Manutenível* - Atualizar um software é mais fácil. Uma pequena modificação vai beneficiar todas as partes que usarem o objeto.
* *Extensível* - O software não é estático. Ele deve crescer para permanecer útil.
* *Reutilizável* - Podemos usar objetos de um sistema que criamos em outro sistema futuro.
* *Natural* - Mais fácil de entender. Você se preocupa mais na funcionalidade do que nos detalhes de implementação.
  
***

**Modificadores de Visibilidade**
Indicam o nível de acesso aos componentes internos de uma classe.
* *public* - a classe atual e todas as outras classes.
* *private* - somente a classe atual.
* *protected* - a classe atual e todas as suas sub-classes.

***

**Pilares da POO**
* [[Encapsulamento]]
* [[Herança]] 
* [[Poliformismo]]
* [[Abstração]]

***
### Princípios de Orientações a Objetos

* **COESÃO** - União harmônica entre uma coisa e outra. Métodos e atributos são harmônicas com a classe. Então coesão é justamente isso, quando você tem uma harmonia entre elementos. Classes não coesas tendem a crescer indefinidamente, o que as tornam difíceis de manter.
* **ENCAPSULAMENTO** - Incluir o proteger alguma coisa em uma cápsula. Encapsulamento é uma forma de manter os objetos das nossas classes protegidos, fornecendo apenas o que é estritamente necessário para o mundo exterior.Classes não encapsuladas permitem violação de regras de negócio, além de aumentarem o acoplamento. 
* **ACOPLAMENTO** - Ação de acoplar. Agrupamento aos pares. Classes acopladas causam fragilidade no código da aplicação, o que dificulta sua manutenção.

***

-   *Coesão*:
    -   Uma classe coesa faz bem uma única coisa
    -   Classes coesas não devem ter várias responsabilidades
-   *Encapsulamento*:
    -   Getters e setters não são formas eficientes de aplicar encapsulamento
    -   É interessante fornecer acesso apenas ao que é necessário em nossas classes
    -   O encapsulamento torna o uso das nossas classes mais fácil e intuitivo
-   *Acoplamento*:
    -   Acoplamento é a dependência entre classes
    -   Acoplamento nem sempre é ruim, e que é impossível criar um sistema sem nenhum acoplamento
    -   Devemos controlar o nível de acoplamento na nossa aplicação



