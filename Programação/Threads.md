
![[Pasted image 20221209162001.png]]

* **java.lang.Thread**

```
new Thread(new Runnable() {
			@Override
			public void run() {
				System.out.println("resposta");
			}
		}).start();
```


* **Operação Atômica**

```
synchronized (this) {
	System.out.println(nome + " Entrando no banheiro");
	System.out.println(nome + " Fazendo coisa rapida");
	try {
		Thread.sleep(5000);
	} catch (InterruptedException e) {
		e.printStackTrace();
	}
	System.out.println(nome + " Dando descarga");
	System.out.println(nome + " Lavando mao");
	System.out.println(nome + " Saindo banheiro");
}

ou

public synchronized void adicionaElementos(String elemento) {
	this.elementos[indice] = elemento;
	this.indice++;
}

```

**Mutex (acrônimo para Mutual Exclusion)** é uma técnica para conceder acesso exclusivo a um dado/recurso compartilhado para apenas um thread, evitando o acesso concorrente.

***
Estados de um thread:
-   **NEW** Uma thread foi criada mas ainda não foi iniciada.
-   **RUNNABLE** A thread está rodando dentro da JVM.
-   **BLOCKED** A thread foi bloqueada pois não conseguiu pegar a chave.
-   **WAITING** A thread está esperando pois foi chamado `this.wait()`.
-   **TIMED_WAITING** A thread está esperando pois foi chamado `this.wait(milis)`.
-   **TERMINATED** A thread está finalizada.

***
Uma thread _daemon_ é uma prestadora de serviços para outras threads. Ela só é usada enquanto as outras threads estão rodando.


