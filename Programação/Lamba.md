Lambda é para interface que tem somente um método e se chama **Interface Funcional**.
Foi criada uma anotação para verificar se é um interface funcional `@FunctionalInterface`.

```
lista.sort((Conta c1, Conta c2) -> {
			return c1.getTitular().compareTo(c2.getTitular());
		});****
```

```
lista.sort((Conta c1, Conta c2) -> c1.getTitular().compareTo(c2.getTitular()));
```

```
lista.sort((c1, c2) -> c1.getTitular().compareTo(c2.getTitular()));
```

```
lista.forEach(conta -> System.out.println(conta));
```

**Predicate** é uma interface funcional do Java 8 que só tem um único método chamado test.

**Sintaxe Lambada** - `(parâmetros) -> { código }`

**Regras**
* se tem somente um parâmetro, não precisa do parênteses.
* se tem mais que um parâmetro, precisa do parênteses e separados por vírgula.
* se só tem uma linha de código, não precisa das chaves.
* se não tem parâmetros, obrigatório por os parênteses.
* se a única linha de código não precisa colocar o retorno.
* se conseguir descobrir o tipo do parâmetro, pode ser omitido o tipo.
