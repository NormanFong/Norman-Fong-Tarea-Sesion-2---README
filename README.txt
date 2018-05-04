-�Por qu� el algoritmo de B�squeda Binaria tiene complejidad logar�tmica?
El Algoritmo de b�squeda binaria es un algoritmo de b�squeda en vectores ordenados
que permite disminuir la complejidad de la b�squeda en dichos vectores. Consiste en
mantener unos �ndices que marcan los l�mites superior e inferior de la parte del
vector que nos queda por analizar. Para calcular la complejidad de este algoritmo, el
n�mero de elementos por analizar es n. Tras la primera divisi�n, el n�mero ser� como
mucho n/2, luego n/4, y as� sucesivamente. Tras una divisi�n i, el n�mero de elementos
ser�, como mucho: \[\frac{n}{2^i}\]
El peor caso se da cuando el elemento buscado no est� en el vector (cuando el n�mero de
elementos a analizar es menor a 1). Por ejemplo, el n�mero de llamadas a realizar es el
n�mero m tal que: [\frac{n}{2^m} < 1\].
Transformando �sta f�rmula a un logaritmo base 2, resulta: \[n < 2^m\], y que:
\[\log n < m\].
Por �sto es que el algoritmo de B�squeda Binaria tiene complejidad logar�tmica.

-�Por qu� el algoritmo de serie Fibonacci tiene complejidad exponencial?
La sucesi�n de Fibonacci es aquella sucesi�n que comienza con los t�rminos 0 y 1, y
continua obteniendo cada t�rmino sumando sus dos anteriores, de esta forma:
0 si n= 0
1 si n= 1
Fib(n-1) + Fib(n-2) si n > 1
En la aplicaci�n de esta sucesi�n como algoritmo, se esta llamando recursivamente a sus
dos anteriores. Cada una de estas llamadas, si es mayor que 1, estar� llamando nuevamente
a sus dos anteriores, de esta forma:
paso 1: 2 ejecuciones
paso 2: 2* (2 ejecucuciones)
paso 3: 2*(2*(2 ejecuciones))
paso k: (2^k) ejecuciones
Por eso es un algoritmo de orden exponencial.

