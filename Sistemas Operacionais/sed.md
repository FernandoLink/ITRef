
##### sed - editor de fluxo para filtragem e transformação de texto
***

Sintaxe Geral: sed 'expressão regular' [arquivo]

| expressão regular | descrição |
|----|----|
| s\/\<texto1\>\/\<texto2\>\/ | substitui o texto1 pelo texto2 |
| y\/\<c1\>\/\<c2\>\/ | substitui caracter c1 por caracter c2 |
| \/\<texto\>\/p | imprime a linha que contenha o texto|
| \/\<texto\>\/d | deleta linhas que contenham o texto|
| \n,md | deleta da linha n até a m|
| 'na\\\<texto\>'| acrescenta após o endereço n informado |
| 'ni\\\<texto\>'| insere antes do endereço n informado |
| 'nc\\\<texto\>'| altera a linha do endereço n informado |
| 'q'| finaliza sed|
| -n '\/\<texto\>\/p'| não mande nada para a saída, a não ser que algo explicitamente o mande fazê-lo|
| -i 's\/\<texto\>\/\<texto\>'| alterar definitivamente o arquivo |
| -i.\<bkp\> 's\/\<texto\>\/\<texto\>'| alterar definitivamente o arquivo original e manter uma cópia no .bkp|
| -r '\<RE\>'| avisa ao sed que serão usados metacaracteres avançados |








