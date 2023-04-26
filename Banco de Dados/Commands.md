***
mongosh

db.help()
sh.help() - *sharding*
rs.help() - *replica*

db.version()
db.hostInfo()
db.getName()
db.stats()
db.listCommands()

show databases
use database
db.createCollection("collection")
show collections
db.collection.drop()
db.dropDatabase()
db.collection.insertOne(json)
db.collection.insertMany([json])
db.collection.find({filter},{projection}).sort({}).limit(5)
db.collection.find().pretty()
db.collection.findOne({})
db.collection.updateOne(filter,json)
db.collection.updateMany(filter,[json])
db.collection.replaceOne(filter,json)
db.collection.deleteOne(filter)
db.collection.deleteMany(filter)
db.getCollectionInfos({name:"collection"})
db.runCommand({listCollections: 1, filter:{name: "contas"}})
db.runCommand({listCollections: 2)
db.runCommand( { collMod: "clientes",
  validator:{
    $jsonSchema: {
    }
})
let collection = { $jsonSchema}
db.collection.find(collection)
db.clientes.find({$nor: [collection]})
db.collection.renameCollection("colection")
db.collection.findAndModify()
db.collection.findOneAndUpdate()
db.collection.findOneAndReplace()
db.collection.findOneAndDelete()
db.alunos.createIndex({localizacao : "2dsphere"})

****
- **Operadores de comparação:** retornam dados com base em comparações de valor ($eq $gt $gte $lt $lte $in).
- **Operadores lógicos:** retornam dados com base em expressões avaliadas como verdadeiras ou falsas ($and $or $nor $not).
- **Operadores de elemento:** retornam dados com base na existência de campo ou tipos de dados ($exist $type).
- **Operadores de matriz:** retornam dados com base nas condições de uma matriz ($all $size $unwind $sortByCount $match $lookup, $unionWith).
- **Operadores de projeção:** especificam os campos retornados por uma operação ($slice). 
- **Operadores Aritméticos:** $rand $round $trunc $multiply $divide
- **Operadores de String:** $concat $split $toLower $toUpper $toString
- **Operadores de Data:** formato ano-mes-dia e fuso horário UTC. $year $month $dayOfWeek $dateToParts
		Usamos o `ISODate()` quando queremos inserir datas ou data e hora.
		O `new Date()` cumpre a mesma função, mas também fornece a data atual do sistema, basta passar o código desta forma: `new Date`.
* **Operadores Acumuladores:** $avg $min $max $count $sum
* **Operadores de Condicional:** $gte $ifNull $switch
 ***
-   **$group:** Agrupa dados com base em um id
-   **$count:** Realiza a contagem de documentos existente em uma coleção
-   **$limit:** Limita a saída de documentos em uma consulta
-   **$sort:** Ordena o resultado de uma consulta de forma crescente ou decrescente
-   **$skip:** Controla a saída inicial dos resultados de uma consulta
-   **$unwind:** Desconstrói um campo de matriz em novos documentos
-   **$match:** Filtra os documentos para retornar em uma consulta
-   **$lookup:** Realiza uma junção entre dados de duas coleções
***
## Operadores de consulta de avaliação:

Esses operadores retornam dados em uma consulta baseada em avaliações de campos individuais ou de toda a coleção.

-   $expr - Permite o uso de expressões de agregação dentro da linguagem de consulta.
-   $jsonSchema - Valida os documentos em relação ao esquema JSON fornecido.
-   $mod - Executa uma operação de módulo no valor de um campo.

## Operadores de consulta geoespacial:

Os operadores geoespaciais permitem que seja realizado consultas baseadas em dados geográficos.

-   $geoWithin: seleciona documentos dentro de um determinado polígono;
-   $near: seleciona documentos baseados em pontos geoespaciais do mais próximo ao mais distante.

## Operadores de consulta bit a bit:

Os operadores de consulta bit a bit são utilizados para realizar operações com base nas condições de posição de um bit.

-   $bitsAllClear: seleciona documentos onde todos os bits especificados são 0.
-   $bitsAllSet: seleciona documentos onde todos os bits especificados são 1.
-   $bitsAnyClear: seleciona documentos onde pelo menos um dos bits especificados é 0.
-   $bitsAnySet: seleciona documentos onde pelo menos um dos bits especificados é 1.
***
*Cursor de Modificação* - .limit() .skip() .sort() count() .distinct() .aggregate()
***
*Docker*

* docker run -d -p 27017:27017 --name my_mongodb -e MONGO_INITDB_ROOT_USERNAME=root -e MONGO_INITDB_ROOT_PASSWORD=pass mongo
* mongosh -u root -p pass --authenticationDatabase admin
* db.getMongo()
* mongodb://root:pass@127.0.0.1:27017/?directConnection=true&serverSelectionTimeoutMS=2000&authSource=admin&appName=mongosh+1.8.0
***
*Import*
mongoimport.exe --host my_mongodb:27017 --db=showbank --collection=Contas --type=csv --headerline --file=file.csv

-   **--db:** Para identificar o banco de dados.
-   **--collection:** Para identificar em qual coleção o arquivo será importado.
-   **--type:** Para informar o tipo do arquivo.
-   **--headerline:** Para indicar que a primeira linha do arquivo CSV é cabeçalho, ou seja, os nomes das colunas.
-   **--file:** Para informar o local onde o arquivo está salvo em seu ambiente.
-   **--jsonArray:** Para indicar que no arquivo existe um array.

***

##### SITES
***
[Operators](https://www.mongodb.com/docs/manual/reference/operator/query/)
