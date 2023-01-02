
| Meta | Nome | Dicas |
|:-----------|------------|-----|
|. |Ponto |Curinga de um caractere
|[] |Lista |Dentro todos são normais, traço é intervalo ASCII
|\[^]  | Lista negada| Sempre casa algo
|? |Opcional |Guloso, 0 ou 1, pode ter ou não
|* |Asterisco |Guloso, 0 ou mais, repete em qualquer quantidade
|+ |Mais |Guloso, 1 ou mais, repete em qualquer quantidade, pelo menos uma vez
|{,} |Chaves |Guloso, número exato, mín., máx., ou uma faixa numérica
|^ |Circunflexo |Casa o começo da linha, especial no começo da ER
|$ |Cifrão |Casa o fim da linha, especial no fim da ER
|\b| Borda |Limita uma palavra (letras, números e sublinhado)
|\ |Escape |Escapa um meta, tira seu poder, escapa a si mesmo \\
|\| |Ou |Indica alternativas, poder multiplicado pelo grupo
|()| Grupo |Agrupa, é quantificável, pode conter outros grupos
|\1| Retrovisor |Usado com o grupo, máx. 9, conta da esquerda para a direita
|\.\*| Curinga |Qualquer coisa, o tudo e o nada
|\?\?| Opcional |Não-guloso, 0 ou 1, casa o mínimo possível
|\*\?| Asterisco |Não-guloso, 0 ou mais, casa o mínimo possível
|\+\?| Mais |Não-guloso, 1 ou mais, casa o mínimo possível
|\{\}\?| Chaves  |Não-guloso, numérico, casa o mínimo possível

-   `?` - zero ou uma vez.
-   `*` - zero ou mais vezes.
-   `+` - uma ou mais vezes.
-   `{n}` - exatamente n vezes.
-   `{n,}` - no mínimo n vezes.
-   `{n,m}` - no mínimo n vezes, no máximo m vezes.