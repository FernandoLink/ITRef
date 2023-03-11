***

*PowerShell possui uma convenção de nomes muito forte, no formato Verb-Noun.* (cmdlet)

* **get-command** - comandos disponíveis.
* **get-command | out-gridview** - comandos disponíveis numa grid view.
* **get-command -name *rename*
* **hostname** - devolve o Computarname.
* **echo $env:path** - mostrar variável de ambiente PATH.
* **$env:path.GetType()** - tipo do retorno do objeto.
* **$env:path.Split(";")** - mostrar variável de ambiente PATH melhor visualizado.
* **$env:path | Get-Member** - help do objeto.
* **alias** - apelidos.
* **get-alias -Name "dir"** - comando dir no powershell.
* **Update-Help** - baixar a ajuda no computador.get
* **-WhatIf** - não executa o comand, somente mostra o que o comando faria.
* **$PROFILE** - exibir a localização do profile do powershell.
* **$PSVersionTable.PSVersion** - mostrar a versão do powershell.
* **new-item $PROFILE** - cria o arquivo de profile.
* **get-executionpolicies** - política de restrições de execução.
* **get-variable** - variáveis globais.
* **$private:variavel**
* **out-file** - gera um arquivo.
* **get-psdrive**
* **enter-pssession** - entrar na sessão powershell de outro servidor.

`get-variable | ? name -like *erro*`

`$servico = Get-Service -Name "UserManager" -ComputerName "DESKTOP-LINK"`

`gci -Recurse -File | Select-Object name | where-object { $_ -like "*bat*" }`

* **FILTER LEFT, FORMAT RIGHT**
`gci -Recurse -File | where-object name -like "*bat*" | select-object  name, length, mode`

* **formatando file size**
`(5434534335 / 1gb).tostring("N2") + "GB"`
`"{0:N2}GB" -f (5434534335 / 1gb)`
`"{0:N2}GB = {1:N2}MB" -f (5434534335 / 1gb), (5434534335 / 1mb)`
`gci -Recurse -File | where-object name -like "*bat*" | select-object  name, { "{0:N2}KB" -f ($_.length / 1kb) }`

* **multiline**
```
gci -Recurse -File `
| where-object name -like "*bat*" `
| select-object  name, { "{0:N2}KB" -f ($_.length / 1kb) }
```

```
gci -Recurse -File |
 where-object name -like "*bat*" |
 select-object  name, { "{0:N2}KB" -f ($_.length / 1kb) }
```

* **Array de Object**
`(1,2,3).gettype()`
`(,1).gettype()`
`@().gettype()`

* **HashTable**
`@{}.GetType().name`
`@{} | get-member`
`(@{} | get-member -name add).definition`

* **Comand interator**
`$computers = 1..5 | % { "Server$_" }

