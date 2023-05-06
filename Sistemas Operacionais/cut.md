***
##### cut - cortar cadeias de caracteres
***

| comando | descrição |
|---|----|
|cut -cn arq | retorna todos os caracteres de posição n |
|cut -cn-m arq| retorna todas as cadeias entre n e m |
| cut -cn- arq | retorna todas as cadeias a partir de n |
|cut -c-m arq | retorna todas as cadeias do n até m|
| cut -fcampo arq | retorna o campo campo |
| cut -fcampoini-campofim arq| retorna campos de campoini a campofim|
| cut -fcampoini- arq | retorna todos os campos a partir de campoini|
|cut -f-campofim arq | retorna todos os campos até o campofim|
|cut -d\<c\>| qual será o separador de campos do arquivo|


Observação: Se não informado o delimitador \<TAB\> é o default.

`cut -c 1-4,15-20 --output-delimiter=";"`

`cut -f 1,5 -d: /etc/passwd`


