
##### ECHO - exibir uma linha de texto
***

|Expressão |Resultado|
|---|---|
|id\+\+ i d\-\- |pós-incremento e pós-decremento de variáveis
|\+\+id \-\-id |pré-incremento e pré-decremento de variáveis
|\*\*| exponenciação
|\* \/ \%| multiplicação, divisão, resto da.divisão/ 
|\+ \- |adição, subtração
|\<\= \>\= \< \>| comparação
|\= \!\= |igualdade, desigualdade
|\&\& |E lógico
|\|\|| OU lógico 

**Exemplo:**

```
flink@PC:~$ var=50
flink@PC:~$ echo $var
50
flink@PC:~$ var=$((var>40 ? var-40 : var+40))
flink@PC:~$ echo $var
10
```



