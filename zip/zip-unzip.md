***
zip arquivo.zip arquivos
zip -r arquivo.zip * (compacta recursivamente)
zip -v arquivo.zip * (verbose)
find . -name "\*.html" | zip -@ arquivos.zip

unzip -l arquivo.zip (listar os arquivos)
unzip -q arquivo.zip (quiet mode)
unzip -d temp arquivo.zip (qual diretório quero descompactar)
unzip arquivo.zip arquivos (descompacta somente os arquivos que vc quer)


