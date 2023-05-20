***

|Comando|Descrição|
|---|---|
|git --help| Ajuda geral do git
|git [comando] --help| Ajuda do comando
|git init| Inicializar um novo repositório Git em um diretório. Cria uma estrutura interna do Git no diretório, incluindo uma pasta oculta chamada ".git". Essa pasta contém todos os arquivos e metadados necessários para rastrear as alterações do projeto.
|git status|Usado para verificar o estado atual do seu repositório Git. 
|git config --local user.name "Seu nome aqui"|Configurar o nome do usuário associado aos commits em um repositório Git específico.
|git config --local user.email "seu@email.aqui"| configurar o endereço de e-mail do usuário associado aos commits no repositório Git específico.
|git branch -m master main| Usado para renomear um branch.
|git add .| Usado para adicionar todas as alterações no diretório de trabalhao ao índice do Git.
|git commit -m "mensagem"| Usado para fazer um commit das alterações preparadas no índice (staging area) para o repositório Git.
|[[git log]]|Usado para visualizar o histórico de commits em um repositório Git.
|[[git config]]|Usado para configurar ou exibir configurações do Git.
|.gitignore|Usado para especificar quais arquivos e diretórios devem ser ignorados pelo Git ao rastrear alterações em um projeto.
|git init --bare |Usado para criar um repositório Git vazio sem um diretório de trabalho. Ao contrário de um repositório Git regular, um repositório bare não contém uma cópia do código-fonte e é geralmente usado como um repositório central para compartilhar código entre vários desenvolvedores.
|[[git remote]]|Usado para gerenciar os repositórios remotos associados a um repositório Git local. Os repositórios remotos são versões do seu projeto que estão hospedadas em servidores externos ou em outros diretórios do sistema.
|[[git clone]] |Usado para criar uma cópia local de um repositório Git remoto. Ele baixa todo o histórico de commits, ramificações e arquivos do repositório remoto e cria uma cópia em seu ambiente local.
|[[git push]]|Usado para enviar as alterações locais de um repositório Git para um repositório remoto. Ele atualiza o histórico de commits do repositório remoto com os commits feitos localmente.
|[[git pull]]|Usado para atualizar o repositório local com as alterações mais recentes do repositório remoto. Ele busca as alterações do repositório remoto e as mescla automaticamente com o branch atual do repositório local.
|git branch|Usado para listar, criar e gerenciar branches (ramificações) em um repositório Git.
|[[git checkout]]|Usado para alternar entre branches (ramificações) existentes ou criar uma nova branch em um repositório Git
|git merge|Utilizado para combinar alterações de um branch em outro.
|git rebase|Usado para reaplicar commits de uma branch em cima de outra branch.
|[[git reset]]|Usado para desefazer commits, mover o branch atual para um commit específico ou desfazer alterações em arquivos.
|git revert|Usado para desfazer commits anteriores, criando um novo commit que reverte as alterações introduzidas por um commit específico. Ao contrário do comando `git reset`, que reescreve o histórico de commits, o `git revert` cria um novo commit que desfaz as alterações do commit original.
|[[git stash]]|Usado para salvar temporariamente as alterações não confirmadas em uma área de armazenamento chamada "stash" e limpar o diretório de trabalho para que você possa alternar para outro branch ou aplicar outras alterações.
|[[git diff]]|Usado para exibir as diferenças entre commits, entre o diretório de trabalho e o índice (staging area), ou entre o diretório de trabalho e um commit específico.
|[[git tag]]|É uma referência a um commit específico em um repositório. As tags são usadas para marcar pontos importantes na linha do tempo do projeto, como versões de lançamento.
|[[git cherry-pick]]|Usado para aplicar um commit específico de um ramo para outro. Ele permite selecionar um único commit e aplicar suas alterações no ramo atual, incorporando essas alterações ao histórico do ramo atual.
|git show|Usado para exibir informações detalhadas sobre um determinado commit.
|[[git bisect]]|Auxilia na localização de um commit específico que introduziu um bug ou causou um problema em seu código.
|git blame|Usado para rastrear a autoria e a última modificação de cada linha de um arquivo.

*Observação:* git comando --help 

**Git Flow***
***
![[Pasted image 20230520164007.png]]

**Hooks**
***
/.git/hooks -> É um diretório especial em um repositório Git que contém scripts de ganchos (hooks) personalizados. Os ganchos são scripts executados automaticamente pelo Git em momentos específicos do ciclo de vida do Git, como antes ou depois de certas ações, como commits, merges, push e outros eventos.

-   [applypatch-msg](https://github.com/git/git/blob/master/templates/hooks--applypatch-msg.sample)
-   [pre-applypatch](https://github.com/git/git/blob/master/templates/hooks--pre-applypatch.sample)
-   [post-applypatch](https://www.git-scm.com/docs/githooks#_post_applypatch)
-   [pre-commit](https://github.com/git/git/blob/master/templates/hooks--pre-commit.sample)
-   [prepare-commit-msg](https://github.com/git/git/blob/master/templates/hooks--prepare-commit-msg.sample)
-   [commit-msg](https://github.com/git/git/blob/master/templates/hooks--commit-msg.sample)
-   [post-commit](https://www.git-scm.com/docs/githooks#_post_commit)
-   [pre-rebase](https://github.com/git/git/blob/master/templates/hooks--pre-rebase.sample)
-   [post-checkout](https://www.git-scm.com/docs/githooks#_post_checkout)
-   [post-merge](https://www.git-scm.com/docs/githooks#_post_merge)
-   [pre-receive](https://www.git-scm.com/docs/githooks#pre-receive)
-   [update](https://github.com/git/git/blob/master/templates/hooks--update.sample)
-   [post-receive](https://www.git-scm.com/docs/githooks#post-receive)
-   [post-update](https://github.com/git/git/blob/master/templates/hooks--post-update.sample)
-   [pre-auto-gc](https://www.git-scm.com/docs/githooks#_pre_auto_gc)
-   [post-rewrite](https://www.git-scm.com/docs/githooks#_post_rewrite)
-   [pre-push](https://www.git-scm.com/docs/githooks#_pre_push)
