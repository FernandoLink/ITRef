
##### SISTEMA
***

|comando| descrição|
|:-----------|-----------|
| logout | encerra de uma vez a sessão do usuário      | 
| ctrl+d | funciona como o logout      | 
| logout | encerra de uma vez a sessão do usuário      | 

##### ARQUIVOS E DIRETÓRIOS
***

| comando | descrição |
|:------------|-----------|
| pwd| exibe o nome do diretório corrente|
|cd              | navegando entre diretórios|
|ls               | listar arquivos|
|cp               | cópia de arquivos|
|mv               | move arquivos e diretórios|
|ln               | estabelece ligação entre arquivos|
|mkdir            | cria um diretório|
|rmdir            | remove um diretório vazio|
|rm               | apaga arquivos e diretórios|
|file            | indicando tipo de arquivo|
|[[grep]]             | localizar cadeira de caracteres em uma entrada definida|
|[[find]]            | localiza arquivo por suas características|
|basename        | devolve o nome de um arquivo recebendo o caminho completo|
|dirname          | devolve o nome do diretório recebendo o caminho completo|
|dir              | lista o contéudo do diretório|
|which| localiza um comando|
|. (ponto)| diretório atual|
|.. (dois pontos) | diretório anterior|
|~ (til)        | diretório home do usuário|
|/ (barra)      | diretório raiz|
|- (hífen)       |último diretório|

##### HELP
***

|comando|descrição|
|:----|---|
| --help | mostra a ajuda do comando |
| help | mostra informações gerais sobre os built-ins do shell |
| man | mais completa documentação do Linux |
| h  | mostra a ajuda do man|
| apropos or man -k | mostra informações sobre um tópico|
| whatis | obtém uma breve descrição de um comando do sistema|
| --version | mostra a versão do comando|
| --usage | ajuda curta do comando (não são todos os comandos)|

##### FILTROS
***

|comando|descrição|
|:----|---|
| cat | exibe conteúdo de arquivos |
| wc | conta caracteres, palavras e/ou linhas de arquivos
| sort | ordena o conteúdo de arquivos
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
| ps | mostra status dos processos em execução|
|kill  | envia sinal a processo
|jobs  | lista processos em background e suspensos
|bg    | passa processo para background
|fg    | traz processo para foreground
|Nohup | executa processo independente de terminal

##### AGENDAR TAREFAS
***

| comando | descrição |
|:-----|-----|
|crontab | instalar, desinstalar ou listar as tabelas usadas pelo programa cron
|cron | agendar a execução de tarefas administrativas
|at | permite que se programem datas e horas para execução de tarefas
|batch | executar tarefas pesadas em segundo plano (background)


  

