***
stdin - canal 0 
stdout - canal 1
stderr - canal 2

Pega a stderr e joga para stdout
`cat /hsdfsdfj 2>&1 > saida.txt`

Pega a stdout e joga para o arquivo, pega a stderr e joga na stdout
`cat /sdjkfh > saida.txt 2>&1`

`find . -name "log*" | zip logs.zip -@`

`zip -@ logs.zip < arqszip`