***

Throwable
- Error
	- OutOfMemoryError
* Exception
	* checked
		* IOException
		* SQLException
		* InterruptedException
	* RuntimeException
		* unchecked
			* NullPointerException
			* IndexOutOfBoundsException
			* ArithmeticException

***
**checked** - Elas precisam ser tratadas explicitamente pelo programador, ou seja, o código precisa incluir uma declaração `try`-`catch` ou um bloco `throws` para lidar com essas exceções.
**unchecked** - Elas não precisam ser tratadas explicitamente pelo programador, ou seja, o código não precisa incluir uma declaração `try`-`catch` ou um bloco `throws` para lidar com essas exceções.
