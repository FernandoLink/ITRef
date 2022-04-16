
| b-l| Nome |Tradução|
|----|-------|-------|
| \a |Alert |Alerta (bipe)
| \b |Backspace| Caractere Backspace
| \e |Escape |Caractere Esc
| \f |Form feed |Alimentação
| \n |Newline |Linha nova
| \r |Carriage return| Retorno de carro
| \t |Htab |Tabulação horizontal
| \v |Vtab |Tabulação vertical

| b-l| Equivalente POSIX |Significa|
|---|---|---|
| \d |\[[:digit:]] |Dígito
| \D |\[\^[:digit:]] |Não-dígito
| \w |\[\[:alnum:]_] |Palavra
| \W |\[\^[:alnum:]_] |Não-palavra
| \s |\[[:space:]] |Branco
| \S |\[\^[:space:]] |Não-branco


| b-l| Significado |Similar|
|---|---|----|
| \a |Alfabeto |\[\[:alpha:]]|
| \A |Não alfabeto |\[\^[:alpha:]]|
| \h |Cabeça de palavra |\[\[\:alpha\]\_]|
| \H |Não cabeça de palavra |\[\^\[\:alpha\:\]\_]|
| \l |Minúsculas |\[\[\:lower\:\]\]|
| \L |Não minúsculas |\[\^\[\:lower\:\]\]|
| \u |Maiúsculas |\[\[\:upper\:\]\]
| \U |Não maiúsculas |\[\^\[\:upper\:\]\]
| \o |Número octal |\[0-7\]
| \O |Não número octal |\[^0-7\]
| \B |Não-borda|
| \A |Início do texto|
| \Z |Fim do texto|
| \l |Torna minúscula|
| \L |Torna minúscula até \E|
| \u |Torna maiúscula|
| \U |Torna maiúscula até \E|
| \Q |Escapa até \E|
| \E |Fim da modificação|
| \G |Fim do casamento anterior|

