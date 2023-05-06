
##### grep (Global Regular Expression Print) 
Pesquisa cadeias de caracteres a partir de uma entrada definida, podendo ou não usar expressões regulares.
***
##### egrep (Extended Global Regular Expression Print)
Idêntico ao grep, porém mais poderoso e mais lento. Esse comando só deve ser utilizado em casos em que seja imprescindível o uso de expressões regulares complexas.
***
##### fgrep (Fast Global Regular Expression Print)
O rapidinho da família, seu uso é indicado para critérios de pesquisa que não envolvem expressões regulares.
***

| comando |  descrição |
|--|--|
| egrep '\^\(i\|I\)' | localizar linha começadas por i ou I |
| grep '\^\[i\|I\]' | localizar linha começadas por i ou I |
|grep -c | conta a quantidade de linhas quem contêm uma determinada cadeia de caracteres|
| fgrep -l | quais são os arquivos que possuem uma determinada cadeira de caracteres|
|grep -l| quais são os arquivo não possuem uma determinada cadeira de caracteres|
|fgrep -v | devolve todas as linhas que não possuem a cadeia pesquisada |
| fgrep -f \<file\>| pesquisa um arquivo procurando por expressões regulares em outro arquivo|
|fgrep -o | devolve somente a parte que casou com a expressão regular |
| grep -An | pega além da linha que casou com a expressão regular, n linhas após |
| grep -Bn | pega além da linha que casou com a expressão regular, n linhas antes|
|grep -i| case insensitive|
| grep -r| recursivo|
| grep -E | expressão regular|
|grep -n| qual linha aparece a palavra|


`grep '[[:digit:]]\+[,\.]\?[[:digit:]]*' *






