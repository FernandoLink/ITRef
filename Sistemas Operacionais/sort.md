***

Utiliza a língua para ordenar
echo $LANG
echo $LC_ALL
echo $LC_COLLATE

Obs.: Se não tiver nada setado utiliza a tabela ASCII por default, no ASCII o maiúsculo vem antes dos minúsculos.

Reverse `sort -r`

Ordena pelo terceiro campo do cut
`cut -c 1-4,5-14,15-20 --output-delimiter=: teste | sort -k 3 -t:`

Tirar as repetidas -u

Arquivo de saída -o