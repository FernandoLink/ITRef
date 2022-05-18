
##### Math
***

|Método|Descrição|Expressão| Resultado|
|:--:|:--:|:--:|:--:|
|PI| Constante PI| Math.PI | 3.1415...|
|pow|Exponenciação| Math.pow(5,2)| 25|
|sqrt|Raiz Quadrada|Math.sqrt(25)|5|
|cbrt|Raiz Cúbica|Math.cbrt(27)|3|
|abs|Valor Absoluto| Math.abs(-10)|10|
|floor| Arredonda para Baixo| Math.floor(3.9)| 3|
|ceil|Arredonda para Cima| Math.ceil(4.2)| 5|
|round|Arredonda Aritmeticamente| Math.round(5.6)| 6|
|random|Gera número aleatório entre 0.0 e 1.0| Math.random()|0.154345|

**Obs.:** Como o random gera um número aleatório entre 0 e 1, caso queira um número entre 5 e 10, utilizar exemplo abaixo.

**Exemplo:**

```
double ale = Math.random();
int n = (int) (5 + ale * (10-5));
```



