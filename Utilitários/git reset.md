***
git reset <opção> <commit>

Existem três opções principais para o `git reset`:

1.  `--soft`: Desfaz o commit, mantendo as alterações do commit desfeito no diretório de trabalho. Os arquivos alterados serão mantidos como alterações não confirmadas (unstaged), permitindo que você faça novos commits com as alterações desfeitas.
    
2.  `--mixed` (padrão): Desfaz o commit e remove as alterações do commit desfeito do índice (staging area). As alterações são mantidas no diretório de trabalho, mas serão mostradas como alterações não rastreadas (untracked). Você precisará adicionar novamente as alterações ao índice e fazer um novo commit.
    
3.  `--hard`: Desfaz o commit e descarta completamente as alterações do commit desfeito. Tanto o índice quanto o diretório de trabalho serão atualizados para refletir o commit desfeito. Tenha cuidado ao usar essa opção, pois as alterações não serão recuperáveis.
    

A opção `<commit>` especifica o commit para o qual você deseja redefinir o branch atual. Pode ser o hash do commit, um nome de branch ou uma referência de commit como `HEAD~1` (o commit anterior ao HEAD).

Aqui estão alguns exemplos de uso do `git reset`:

-   `git reset --soft HEAD~1`: Desfaz o último commit, mantendo as alterações do commit desfeito no diretório de trabalho.
-   `git reset --mixed HEAD~1`: Desfaz o último commit e remove as alterações do commit desfeito do índice.
-   `git reset --hard HEAD~1`: Desfaz o último commit e descarta completamente as alterações do commit desfeito.