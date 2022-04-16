
|Metacaractere| Significado |Dica|
|---|----|---|
|(?#texto) |Texto é um comentário||
|(?:ER) |Grupo fantasma, retrovisor não conta||
|(?=ER) |Casa se ER casar adiante |\=\=|
|(?!ER) |Casa se ER não casar adiante |\!\=|
|(?<=ER) |Casa se ER casar antes |← \=\=|
|\(\?\<!ER) |Casa se ER não casar antes |← \!\=|
|\(\?\<nome>ER) |Nomeia parte de uma ER||
|(?letra) |Letra é um modificador: imsxL||
|(?{código}) |Executa código Perl||
|(?(cond)s\|n) |If-then-else||

