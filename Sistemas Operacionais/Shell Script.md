
| comando | descrição |
|:----|----|
|\#      | comentário
|#!     | entende que é o caminho (path) para o interpretador que será usado por este |script (ex. #!/bin/bash);
| echo  | mostra a linha de texto
|\      | ignora um e somente um caracter que segue a barra invertida
|'      | todos os caracteres entre apóstrofos são ignorados
|"      | entre aspas o shell ignora o seu significado
|\`      | são usadas para avisarmos ao shell que o que está entre elas é um comando
|stdin  | entrada padrão, normalmente teclado
|stdout | saída padrão, normalmente terminal
|\>      | redireciona a saída de uma comando para um especificado
|\>>     | redireciona a saída de um comando para um arquivo especificado, anexando-o ao seu fim
|2>     | redireciona os erros gerados por um comando para o arquivo especificado
|<      | avisa ao shell que a entrada padrão não será o teclado, mas sim o arquivo especificado
|<<     | indica ao shell que o escopo de um comando começa na linha seguinte e termina quando  encontra uma linha cujo conteúdo seja unicamente o label que segue o sinal<<
|\|      | direciona a saída de um comanda para a entrada de outro
|tee   | captura a saída de um comando com pipe, copiando o que está entrando no tee para a saida padrão e outro comando ou arquivo
|\$$     | representa o pid (process identification)
|ed     | editor de text orientado a linha
|sed    | editor para filtrar e transformar texto

  
  
  
  

