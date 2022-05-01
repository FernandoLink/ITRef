
### if
O comando if do shell, no seu formato geral, não testa uma condição, mas sim se uma instrução foi executada com sucesso ou não, isto é, se o código de retorno da instrução foi igual a zero ou não.
***

**Sintaxe**
```
if <comando>                 # Se <comando> for bem sucedido ($? = 0)...
then                         # Então
	<comando>                # Execute
	<comando>                # Estes
	<...>                    # Comandos
else                         # Senão ($? != 0)...
	<comando>                # Execute
	<comando>                # Os outros
	<...>                    # Comandos
fi                           # Fim do teste condicional
```

**Obs.:**
Caso queira que não mostre o resultado do seu comando basta direcionar para o /dev/null.

**Exemplo
```
if expr $1 + 1 > /dev/null 2> /dev/null    # Resultado de expr e erro que irão para /dev/null
then
	echo Eh um numero 
else
	echo Nao eh um numero 
fi
```

**Obs.:**
Substituição ao comando test \<expressao\>, pode ser, simplesmente escrito \[ \<expressao\> \]

**Exemplo**
```
#!/bin/bash
#
# vira - vi resguardando arquivo anterior
#
if [ "$#" -ne 1 ]
then
        echo "Erro -> Uso: $0 <arquivo>"
        exit 1
fi
Arq=$1
if [ ! -f "$Arq" ]    # O arquivo não existe, logo como salva-lo?
then
        vi $Arq
        exit 0
fi
if [ ! -w "$Arq" ]    # Sera que tenho permissao de gravação no arquivo?
then
        echo "Nao perca seu tempo, voce nao conseguira sobregravar $Arq"
        exit 2
fi
cp $Arq $Arq~
vi $Arq
exit 0
```


**And**
```
if [ "$sexo" != 1 -a "$sexo" != 2 ]
then
	echo "Sexo invalido"
fi
```

**Or**
```
if [ "$sexo" -lt 1 -o "$sexo" -gt 2 ) 
then 
	echo "Sexo invalido"
fi
```

**Parênteses (precedência)**
```
if [ \( $sexo -eq 1 -o $sexo -eq 2 \) -a \            # A última \ informa que linha continua
	 \( $nome= joao -o $ nome = maria \) ]            # As outras incluem interpretação dos ()
```

