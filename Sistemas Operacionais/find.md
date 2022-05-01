

* find . -name 'index.html'
* find . -name '*.html'
* find . -not -name '*.html'
* find . -regex 'RE'
* find . -iregex - ignorar maiúsculas e minúsculas
* find . -name -type * - somente arquivos
* find . -user usuário

**Exemplos**

```
find . -type -f -exec grep -l param {} \;
find . -user cara -exec rm -f {} \;       # -user cara significa todos arqs. cujo dono é cara
```


