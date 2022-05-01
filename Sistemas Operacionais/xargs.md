
##### xargs
Construir listas de parâmetros e passá-las para a execução de outros programas ou instruções.
***

|opção| descrição|
|---|---|
|\-i| substitui o par de chaves ({}) pela cadeia recebida|
|\-nNum| manda o máximo de parâmetros recebidos, até o máximo de Num para o comando a ser executado|
|\-lNum| manda o máximo de linhas recebidas, até o máximo de Num para o comando a ser executado
|\-p| mostra a linha de comando montada e pergunta se deseja executá-la|
|\-t| mostra a linha de comando montada antes de executá-la|


```
xargs [comando [argumento]]
```

**Obs.:** caso o comando seja omitido, será usado por default o [[echo]].

