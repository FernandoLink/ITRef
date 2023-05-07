***
##### SISTEMA
***

|comando| descrição|
|:-----------|-----------|
| logout | encerra de uma vez a sessão do usuário      | 
| ctrl+d | funciona como o logout      | 
| logout | encerra de uma vez a sessão do usuário      | 
|hostname|mostra o hostname|
|uname -a|mostra todas as informações do sistema|
|whoami| mostra usuário conectado|
|ps -p \$\$|tipo de shell|
|lshw| informações hardware|
|free| memória|
|cpu-info| cpu|
|df| filesystem disk|
|du| file space usage|
| dmesg| log do kernel|

##### ARQUIVOS E DIRETÓRIOS
***

| comando | descrição |
|:------------|-----------|
| pwd| exibe o nome do diretório corrente|
|cd              | navegando entre diretórios|
|cd - | navegando para o diretório anterior|
|ls               | listar arquivos|
|[[cp]]               | cópia de arquivos|
|mv               | move arquivos e diretórios|
|ln               | estabelece ligação entre arquivos|
|mkdir            | cria um diretório `mkdir -pv d{1,2,3}/c{1,2,3}`|
|rmdir            | remove um diretório vazio `rmdir -pv d{1,2,3}/c{1,2,3}`|
|rm               | apaga arquivos e diretórios|
|file            | indicando tipo de arquivo|
|[[grep]]             | localizar cadeira de caracteres em uma entrada definida|
|[[find]]            | localiza arquivo por suas características|
|basename        | devolve o nome de um arquivo recebendo o caminho completo|
|dirname          | devolve o nome do diretório recebendo o caminho completo|
|dir              | lista o contéudo do diretório|
|. (ponto)| diretório atual|
|.. (dois pontos) | diretório anterior|
|~ (til)        | diretório home do usuário|
|/ (barra)      | diretório raiz|
|- (hífen)       |último diretório|
|touch| cria arquivo/diretório ou muda a data de criação caso já exista|
| more| paginar - ! roda um comando - v abre o vi|
|less| paginar mas pode andar com as setas|
| [[cut]]| extrai pedaço da linha do arquivo|
|[[paste]]| merge linhas de arquivos|
| type | perguntar tipo do comando `type -a pwd`|
|locate| acho arquivos `locate -e mostra`|
|updatedb| atualiza o database do locate, tem que rodar como root|
|uniq| remove as linhas repetidas em sequencia|


##### HELP
***

|comando|descrição|
|:----|---|
| --help | mostra a ajuda do comando |
| help | mostra informações gerais sobre os built-ins do shell |
| man | mais completa documentação do Linux `man -k ascii` |
| h  | mostra a ajuda do man|
| apropos or man -k | mostra informações sobre um tópico|
| whatis | obtém uma breve descrição de um comando do sistema|
| --version | mostra a versão do comando|
| --usage | ajuda curta do comando (não são todos os comandos)|
|whereis| localiza aonde estão binários, fontes e man|
|which| localiza um comando `which -a pwd`|

##### FILTROS
***

|comando|descrição|
|:----|---|
| cat | exibe conteúdo de arquivos |
| wc | conta caracteres, palavras e/ou linhas de arquivos
| [[sort]] | ordena o conteúdo de arquivos
| head | exibe o início dos arquivos
| tail | exibe o final dos arquivos

##### SEGURANÇA
***

| comando | descrição |
|:-------|--------|
|passwd | altera a senha do usuário;                                  |
|chown| troca o dono do arquivo;
|chgrp | troca o grupo do arquivo
|dono(u) | o usuário dono do grupo
|group(g) | o grupo a que pertence o arquivo
|outro(o) | outros usuários que não sejam o dono e nem pertençam ao grupo

##### USUÁRIOS
***

| comando | descrição |
|:------|-------|
|who    | exibe informações sobre usuários ativos e alguns dados do sistema
|id     | informa os identificadores dos usuários
|finger | exibe informações mais detalhadas sobre os usuários
|chfn   | permite que o usuário altere as suas informações do finger
|groups | informa os grupos aos quais o usuário pertence
| groupadd| adicionar grupo
|useradd| adicionar vários usuários
|adduser| adicionar usuário único
|userdel| deletar usuário (-r)
| usermod| modifica a conta do usuário
| groupdel| deletar grupo
|sudo| executa comando como root


###### DATA E HORA
***

| comando | descrição |
|:----|----|
|date | mostra e acerta data/hora
|cal  | exibe o calendário

##### BACKUP
***

|comando|descrição|
|:-----|------|
|tar        | para agrupar vários arquivos em somente um|
|compress   | é o utilitário de compressão de arquivos padrão do unix|
|uncompress | descomprime arquivos compactados pelo compress|
|zcat       | permite visualizar o contéudo de arquivos compactados com compress|
|gzip       | é o utilitário de compressão de arquivos padrão do linux|
|gunzip     | descomprime arquivos compactado pelo gzip|

##### CONTROLE DE EXECUÇÃO
***

| comando | descrição |
|:-----|------|
| [[ps]] | mostra status dos processos em execução|
|pstree| ps no formato de árvore|
|kill  | envia sinal a processo|
|killall| mata todos os processos com o nome tal|
|jobs  | lista processos em background e suspensos|
|bg    | passa processo para background|
|fg    | traz processo para foreground|
|nohup | executa processo independente de terminal|
|top|processos rodando, top -u link|
|htop|processos rodando|
|&| joga diretamente para background|
|sh| interpretador de comandos|


##### AGENDAR TAREFAS
***

| comando | descrição |
|:-----|-----|
|crontab | instalar, desinstalar ou listar as tabelas usadas pelo programa cron
|cron | agendar a execução de tarefas administrativas
|at | permite que se programem datas e horas para execução de tarefas
|batch | executar tarefas pesadas em segundo plano (background)

##### AMBIENTE
***

|comando|descrição|
|--|--|
|[[echo]]| mostra linha de texto|
|set| informa uma lista de todas as variáveis locais, variável de ambiente e funções do shell `set -o emacs` `set -o vi`|
|unset| apaga uma variável de ambiente da memória|
|printenv| imprime as variáveis de ambiente|
|export| exporta as variáveis criadas para todos os processos filhos do shell|
|env| variáveis de ambiente|
|echo $HOME| diretório do usuário|
|echo $LOGNAME| login name|
|echo $UID| user identification|
|echo $EDITOR| editor padrão|
|echo $PS1|definição do prompt |
|echo $PS2|definição do prompt secundário|
|bash| executar um script|
|history|histórico|
|echo $HISTFILE| aonde está gravando o histórico|
| echo $PATH| caminho dos executáveis|
| hash| lembrar ou mostrar a localização dos programas|
|builtin| executa shell builtins |
|echo $?| resultado do último comando executado|
| echo $MANPATH| aonde procurar os manuais ou /etc/manpath.config|
|manpath| path do man|
|groff| converte o man|


-   *"Ctrl+C"*: interrompe a execução do comando atualmente em execução no terminal. Isso é útil se você precisar parar um processo que esteja em execução, como um script que esteja demorando muito para executar. Ao pressionar "Ctrl+C", o processo é encerrado e você retorna ao prompt do terminal.
    
-  *"Ctrl+D"*: envia o caractere EOF (end-of-file) para o processo em execução. Se você estiver executando um comando que espera entrada de dados do usuário, como o comando "cat", pressionar "Ctrl+D" indicará ao comando que não há mais dados para ler e ele encerrará a execução.
    
-   *"Ctrl+Z"*: suspende o processo em execução no terminal. Isso é útil se você precisar interromper temporariamente um processo para executar outro processo e, em seguida, retornar ao processo original. Ao pressionar "Ctrl+Z", o processo é suspenso e você retorna ao prompt do terminal. Você pode retomar a execução do processo em segundo plano usando o comando "bg" (execução em segundo plano) ou "fg" (execução em primeiro plano).
















