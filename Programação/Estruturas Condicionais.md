
##### Estruturas Condicionais
***
**Condição Simples**

```
if (var > 9) {
	System.out.println("Variável maior que 9");
}
```

**Condição Composta**

```
if (var > 9 ) {
	System.out.println("Variável maior que 9");
} else {
	System.out.println("Variável menor ou igual a 9");
}
```

**Condições Encadeadas

```
if (idade < 16) {
	System.out.println("Não vota!");
} else {
	if (((idade >= 16) && (idade < 18)) || (idade > 70)) {
		System.out.println("Voto opcional!");
	} else {
		System.out.println("Voto obrigatório!");
	}
}	

ou

if (idade < 16) {
	System.out.println("Não vota!");
} else if (((idade >= 16) && (idade < 18)) || (idade > 70)) {
	System.out.println("Voto opcional!");
} else {
	System.out.println("Voto obrigatório!");
}
```

**Condições de Múltipla Escolha

```
switch(pernas) {
	case 1:
		tipo = "Saci";
		break;
	case 2:
		tipo = "Bípede";
		break;
	case 4:
		tipo = "Quadrúpede";
		break;
	case 6:
	case 8:
		tipo = "Aranha";
		break;
	default:
		tipo = "ET";
}
```

