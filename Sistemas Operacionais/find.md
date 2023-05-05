***

* find . -name 'index.html'
* find . -iname *conf
* find . -name '*.html'
* find . -not -name '*.html'
* find . -regex 'RE'
* find . -iregex - ignorar maiúsculas e minúsculas
* find . -name -type * - somente arquivos
* find . -user usuário
* find . -group group
* find . -amin -5 (acessados nos últimos 5 dias)
* find . -mtime -2 (modificados nos últimos 2 dias)
* find . -ctime -1 
* find . -size +100M
* find -type d -name "*user*"
* find -inum inode (pode ser usado para ver os links simbólicos de um diretório)
* find -name "log" -name "2006" (é um and)
* find -name "log" -o -name "2016"
* find -name "log" -a -name "2016"
* find (-name "log" -o -name "2016" ) -a -name "018*"
* find -name "log" ! -name "2016"
* find -name "log" -exec ls -l {} \;   (com o resultado do find executa um ls)
