***
-   **Padrão de referência Pai**
```php
db.Pai.insertMany( [
   { _id: "Programação", parent: "Categoria" },
   { _id: "Banco de dados", parent: "Categoria" },
   { _id: "Categoria", parent: "Livraria" },
   { _id: "Autor", parent: "Livraria" },
   { _id: "Livraria", parent: null }
] )
```

-   **Padrão de referência Filho**
```php
db.Empresa01.insertMany( [
   { _id: "Programação", children: [] },
   { _id: "Banco de dados", children: [] },
   { _id: "Categoria", children: [ "Programação", "Banco de dados" ] },
   { _id: "Autor", children: [] },
   { _id: "Livraria", children: [ "Categoria”, "Autor" ] }] )
```

-   **Padrão de array de ancestrais**
```php
db.ancestrais.insertMany( [
  { _id: "Programação", ancestors: [ "Livraria", "Categoria" ], parent: "Categoria" },
  { _id: "Banco de dados", ancestors: [ "Livraria", "Categoria" ], parent: "Categoria" },
  { _id: "Categoria", ancestors: [ "Livraria" ], parent: "Livraria" },
  { _id: "Autor", ancestors: [ "Livraria" ], parent: "Livraria" },
  { _id: "Livraria", ancestors: [ ], parent: null }] )
```

* **Padrão de caminhos materializados**
```php
db.Materializados.insertMany( [
 { _id: "Livraria", path: null },
 { _id: "Autor", path: "Livraria" },
 { _id: "Categoria", path: "Livraria" },
 { _id: "Programação", path: "Livraria", "Categoria" },
 { _id: "Banco de dados", path: "Livraria", "Categoria" }
] )
```

-   **Padrão de conjuntos aninhados**
```php
db.aninhados.insertMany( [
       { _id: "Livraria", parent: 0, left: 1, right: 10 },
       { _id: "Categoria", parent: "Livraria", left: 2, right: 7 },
 { _id: "Autor", parent: "Livraria", left: 8 , right: 9 },
 { _id: "Banco de dados", parent: "Categoria", left: 3, right: 4 },
       { _id: "Programação", parent: "Categoria", left: 5, right: 6 }       
       ] )
```