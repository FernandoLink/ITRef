

##### test
Usado para testar condições.
Avalia <expressão> e, se o resultado for verdadeiro, gera o código de retorno ($?) igual a zero; caso contrário, será gerado um código de retorno diferente de zero.
***

**Exemplo***
```
if test $# = 0                            # Estou recebendo um parâmetro ou não?
then
        echo Faltou informar a resposta   # Não recebi o tal do parâmetro
        exit 1                            # Encerro o programa com o código de retorno diferente de 0
fi
resp=$1
if test "$resp" = N
then
        echo Ela nao deixa...
elif test "$resp" = S
then
        echo Oba, ela deixou!!!
else
        echo Acho que ela esta na duvida.
fi
```

**Testes de condição arquivos**
|opções| verdadeiro ($?=0) se arquivo existe e:|
|--|--|
|-r arquivo| tem permissão de leitura.|
|-w arquivo| tem permissão de gravação.|
|-x arquivo| tem permissão de execução.|
|-f arquivo| é um arquivo regular.|
|-d arquivo| é um diretório.|
|-u arquivo| seu bit set-user-ID está ativo.|
|-g arquivo|seu bit set-group-ID está ativo.|
|-k arquivo| seu sticky bit está ativo.|
|-s arquivo| seu tamanho é maior que zero.|

**Testes com cadeira de caracteres**
|opções | é verdadeiro ($? = 0) se:|
|--|--|
|-z cad1 | o tamanho de cad1 é zero.|
|-n cad1| o tamanho da cadeia cad1 é diferente de zero.|
|cad1 = cad2 | as cadeias cad1 e cad2 são idênticas.|
|cad1| cad1 é uma cadeia não nula.|

**Testes com inteiros**
|operando| é verdadeiro ($? = 0) se: |significado:|
|--|--|--|
|i1 -eq i2|i1 igual a i2| equal to|
|i1 -ne i2| i1 diferente de i2| not equal to|
|i1 -gt i2|i1 maior que i2 | greater than|
|i1 -ge i2| i1 maior ou igual a i2| greater or equal|
|i1 -lt i2 | i1 menor que i2 | less than|
|i1 -le i2| i1 menor ou igual a i2| less or equal|

