
##### pipe
***

**Exemplos**

```
ls -l arq
echo $?   # caso retorno 0 indica que comando anterior foi bem sucedido, diferente de 0 mal sucedido
```

```
date | grep arq | wc -l
echo ${PIPESTATUS[*]}   # mostra retorno dos três comando
echo ${PIPESTATUS[n]}   # mostra retorno um a um, onde n é a sequência do comando anterior (1|2|3)
```

