
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
|<<     | indica ao shell que o escopo de um comando começa na linha seguinte e termina quando  encontra uma linha cujo conteúdo seja unicamente o label que segue o sinal<<|
| <<<| alimenta a entrada primária (stdin) do comando|
|\|      | direciona a saída de um comanda para a entrada de outro
|tee   | captura a saída de um comando com pipe, copiando o que está entrando no tee para a saida padrão e outro comando ou arquivo
|\$$     | representa o pid (process identification)
|[[ed]]     | editor de text orientado a linha
|[[sed]]    | editor para filtrar e transformar texto|
|[[cut]]| cortar cadeia de caracteres|
| [[paste]]| junta cadeia de caracteres|
|[[tr]]| traduz, transcreve ou transforma cadeira de caracteres|
|[[expr]]| execução de operações aritméticas|
|[[bc]]| calculadora|
|uniq| quando desejamos trabalhar com os registros duplicados de uma entrada|

##### VARIÁVEL
O nome de uma variável é iniciado por uma letra ou um sublinhado, seguido ou não por quaisquer caracteres alfanuméricos ou caracteres sublinhado.
Para armazenar ou atribuir valor a uma variável, basta colocar o nome da variável, um sinal de igual colado ao nome escolhido e, colado ao sinal de igual, o valor estipulado. 

**Exemplo:
```
$ variavel=qqcoisa # armazena qqcoisa em variável
$ contador=0       # coloca zero na variável contador
$ vazio=           # cria a variável com o valor null (NULL)
```

Para exibir o conteúdo das variávels devemos preceder o seunome por um cifrão ($).

**Exemplo:
```
$ echo $variavel    # mostra o conteúdo da variável
$ echo ${variavel}1 # mostra o valor da variável, e colocamos o 1 a seguir
```

##### PASSAGEM DE PARÂMETROS PARA O SCRIPT
Para passar parâmetros é somente necessário passar os parâmetros separados por espaço em branco.

**Exemplo:
```
$ programa parm1 parm2 parm3 ... parmn
```

Os parâmetros passados dão origem dentro do programa que os recebe, às variáveis $1, $2, $3, ...$n.

* $0 - recebe o nome do script.
* $# - recebe a quantidade de parâmetros passados para o script.
* $* - contêm o conjunto de todos os parâmetros separados por espaços em branco.

Como o script só reconhece 9 argumentos passados por parâmetro, o comando ***shift*** pode auxiliar para pegar os parâmetros além do nono.

**Exemplo:
```
echo O programa $0 recebeu $# parâmetros
echo $1
echo $2
shift 10              # os 10 primeiros parâmetros foram excluídos
echo $1               # o décimo primeiro se transforma no primeiro
```





