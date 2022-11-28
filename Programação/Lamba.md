

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
lista.forEach((conta) -> System.out.println(conta));
```

