Um objeto que criamos para encapsular uma função ou método.
As classes anônimas facilitam um pouco a criação desses objetos.

```
// Function Object
		lista.sort(new Comparator<Conta>() {

			@Override
			public int compare(Conta c1, Conta c2) {
				return Integer.compare(c1.getNumero(), c2.getNumero());
			}
		});
```

