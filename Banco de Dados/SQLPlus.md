
##### SQLPlus
***
Executar comandos SQL e PL/SQL tipo linha de comando.

**Conexão:** sqlplus user/password@connection

| Comando | Descrição |
|---|---|
|VARIABLE \<nome_variável\> \<tipo> \= \<conteúdo da variável\>| Criar variável.|
|:| Para acessar a variável colocar : antes do nome da variável criada com o comando variable.| 
| SET PAGESIZE \<num\>| Setar o número de linhas printadas na saída em uma página.|
|SET LINESIZE \<num\>| Setar o número de caracteres que mostram em uma linha antes da quebra de linha.|
|\&| Para substituir uma variável temporariamente na sessão.|
|\&\&| Para substituir uma variável definitivamente na sessão e não solicitar quando for utilizar a variável novamente.|
|SPOOL \[stdout/stderr\] \[on/off\] to \[nome_arq\]|Enviar output para um arquivo. Se arquivo não existe cria, se existe sobrescreve. Não cria diretório.|
| DEFINE \<nome_variável\> = \<conteúdo da variável\>| Define variável a ser utilizada pelo & sem necessidade de ser informada.|
|UNDEFINE \<nome_variável\>| Reseta conteúdo e solicita novamente a entrada do conteúdo via &.|
|PROMPT \<msg\>| Envia uma mensagem ou linha em branco caso a mensagem seja omitida.|
|ACCEPT \<var\> \<tipo\> PROMPT \<msg\>| Lê uma linha e armazena para ser utilizada pelo &.|
| SHOW ALL | Mostra todas variáveis do sistema e da sessão.|
| CONN or CONNECT user/password@connection user@connection/password| Conecta no oracle.|
|DISCONNECT| Desconecta a sessão.|
|HOST or HOST cmd| Executa comando do sistema operacional sem deixar o sqlplus, exit volta para o sqlplus.|
|CL SCR or CLEAN SCREEN| Limpa a tela.|
|SET var_system value | Alterar variáveis de sistema.|
|HELP SET\/INDEX| Ajuda do comando SET ou INDEX.|
| SET UNDERLINE 'caracter'| Seta o caracter entre o header e o conteúdo do resultado.|
| SET HEADING \[on/off\]| Mostra ou não o header.|
| SET SQLPROMPT "texto"| Muda o prompt da sessao.|
| SET FEEDBACK num | Exibe o número de registros devolvidos por uma consulta quando uma consulta seleciona pelo menos n registro|
| SET VERIFY \[on\/off\]| Lista instrução SQL antes e depois da substituição de variáveis.|
|SET TIMING \[on\/off\]| Controla a exibição das estatísticas de tempo.|
|EXIT| Sai do sqlplus.|
| \/| Executa o comando anterior.|
| SET SQLTERMINATOR 'char'| Define o caractere usado para terminar e executar a instrução sql.|
|SET SERVEROUTPUT \[on\/off\]| Controla a saída (ou seja, dbms_output.put_line) de procedimentos armazenados ou blocos PL/SQL.|
|LIST or L num| Lista um ou mais linhas do SQL buffer.|
|EDIT file_name| Convoca um editor de texto do sistema operacional sobre o conteúdo do arquivo especificado ou sobre o contéudo do buffer.|
| COLUMN attrib| Especifica os atributos de exibição para uma determinada coluna.|
| SET COLSEP text | Define o texto ou caractere a ser impresso entre as linhas selecionadas.|
|INPUT or I text| Adiciona uma ou mais linhas de texto após a linha atual no buffer.|
| CHANGE or C /de/para | Procura o de no buffer e troca pelo para.|
|DEL num| Deleta a linha especificada no num do buffer da instrução PL/SQL.|
|APPEND or A text| Adiciona text especificado ao final da linha atual no buffer.|
|SAVE filename| Salva o conteúdo do buffer sql em um script de sistema operacional.|
|GET filename|Carrega um arquivo do sistema operacional para o buffer.|
|PASSWORD| Mudar senhar.|
|PRINT var| Exibe os valores atuais das variáveis.|
|SET AUTOPRINT \[on\/off\]| Imprime automaticamente qualquer variável.|
|SET MARKUP HTML \[on\/off\]| Produz o resultado do sql em HTML.|
| SET CMDSEP \[on\/off\]| Habilita/Desabilita e define o caractere separador para colocar vários comandos na mesma linha.|
| SET SQLCASE \[mixed \| lower \| upper\] | Converte o case do comando SQL de acordo com o definido. Não altera o buffer SQL.|
| SET SQLPREFIX char | Define o caractere de prefixo para executar um comando a parte sem afetar o SQL.|
|SET RECSEPCHAR char | Define o caractere a ser exibido para separar os registros.|
| SET RECSEP \[wrapp \| each \| off\] | Define a forma do separador de registro.|
|SET NULL text| Define o texto a ser exibido sempre que um valor nulo ocorre no resultado de uma comando SQL.|
|SET NUMWIDTH num | Define a largura padrão para a exibição de números.|




