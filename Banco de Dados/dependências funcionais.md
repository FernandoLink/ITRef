***
Dependências funcionais são restrições aplicadas sobre atributos e ocorrem quando um atributo determina exclusivamente outro atributo. 
Ou seja, quando um atributo depende de outro para que a sua existência faça sentido.

Ex.: CPF -> nome

O atributo que determina o valor é chamado de **determinante**. 
O outro atributo é chamado de **dependente**.

* *Dependência funcional parcial* só ocorre quando existir um chave primária composta na tabela. E os atributos dependem de somente de parte da chave primária composta.
* *Dependência funcional total* só ocorre quando existe um chave primária composta na tabela. E os atributos dependem de toda a chave primária composta.
* *Dependência Funcional Transitiva* ocorre quando um atributo não chave não depende da chave primária, nem parcialmente, mas depende de outro atributo não chave.