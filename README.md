# M05_UF2_P2_SantiagoHijarAnoro 
Computer Information
CPU name	Intel(R) Core(TM) i7-8550U
CPU speed	1.80GHz   1.99 GHz
CPU threads	8
Memory amount	8,00GB
Memory speed	2133
 
Algorithm 1
Basic information
Name
BubbleSort
Complexity

	Average	Best case	Worst case
When	NA	Si los números ya están ordenados en orden ascendente	Si los números ya están ordenados en orden descendente
Complexity	O(n²)	O(n)	O(n²)

References
https://www.happycoders.eu/algorithms/bubble-sort/

How does it work
Bubble sort es un algoritmo de clasificación simple. Este algoritmo de clasificación es un algoritmo basado en la comparación entre cada par de elementos adyacentes y los intercambia si no están en orden.

Benchmark

	1.000u	10.000u	100.000u
Unsorted	8 ms
81044 ticks	462 ms
4622769 ticks	59768ms
597680837ticks
Ascending	5 ms
52431 ticks	263 ms
3806886ticks	38928ms
389282885ticks
Descending	6 ms
61578 ticks	388ms
3883303ticks	56312ms
563124803ticks)
 
Algorithm 2
Basic information
Name
BubbleSortEarlyExit
Complexity

	Average	Best case	Worst case
When	NA	El mejor caso para la ordenación de burbuja ocurre cuando la lista ya está ordenada o casi ordenada.	El peor caso absoluto para la ordenación de burbujas es cuando el elemento más pequeño de la lista está en el extremo más grande.
Complexity	O(n²)	O(n)	O(n²)

References
https://www.sparknotes.com/cs/sorting/bubble/section1/
How does it work
BubbleeSortEarlyExit El mejor caso para la ordenación de burbuja ocurre cuando la lista ya está ordenada o casi ordenada. En el caso de que la lista ya esté ordenada, la clasificación de burbujas terminará después de la primera iteración, ya que no se realizaron intercambios.

Benchmark

	1.000u	10.000u	100.000u
Unsorted	5 ms
56062 ticks	487 ms
4871260 ticks	72141 ms
721419199 ticks
Ascending	0 ms
43 ticks	0ms
402ticks	0 ms
5470 ticks
Descending	5 ms
50094 ticks	388ms
3883303ticks	57679 ms
573797615 ticks
 
Algorithm 3
Basic information
Name
QuickSort
Complexity

	Average	Best case	Worst case
When	NA	Quicksort logra un rendimiento óptimo si siempre dividimos los arrays y subarrarrays en dos particiones de igual tamaño.	En la práctica, el intento de ordenar una matriz preclasificada en orden ascendente o descendente utilizando la estrategia de pivote, "elemento derecho,", fallaría rápidamente debido a un StackOverflowException, ya que la recursividad tendría que ser tan profunda como grande sea la matriz.
Complexity	O (n log n)	O(n log n)	O(n²)

References
https://www.happycoders.eu/algorithms/quicksort/

How does it work
Quicksort funciona según el principio de "divide y vencerás":
Primero, dividimos los elementos a clasificar en dos secciones: una con elementos pequeños y otra con elementos grandes .
El llamado elemento de pivote determina qué elementos son pequeños y cuáles son grandes. El elemento pivote puede ser cualquier elemento de la matriz de entrada. 
La matriz ahora se reorganiza de modo que: los elementos que son más pequeños que el elemento pivote terminan en la sección izquierda, los elementos que son más grandes que el elemento pivote terminan en la sección derecha, el elemento de pivote se coloca entre las dos secciones que también es su posición final

Benchmark

	1.000u	10.000u	100.000u
Unsorted	0 ms
3925 ticks	1 ms
15330 ticks	35 ms
165681ticks
Ascending	0 ms
457 ticks	0 ms
5281 ticks	11 ms
114805 ticks
Descending	0 ms
463 ticks	0 ms
5509 ticks	11 ms
 112966 ticks

 

Algorithm 4
Basic information
Name
InsertionSort
Complexity

	Average	Best case	Worst case
When	NA	Si los elementos ya aparecen ordenados, hay precisamente una comparación en el bucle interno y ninguna operación de intercambio.	En el peor de los casos, los elementos se ordenan completamente de forma descendente al principio. En cada paso, todos los elementos del subarreglo ordenado deben, por lo tanto, desplazarse hacia la derecha para que el elemento a ordenar, que es más pequeño que todos los elementos ya ordenados en cada paso, pueda colocarse al principio.
Complexity	O(n²)	O(n)	O(n²)

References
https://www.happycoders.eu/algorithms/insertion-sort/

How does it work
Insertion Sort es un algoritmo de ordenación que toma un elemento a la vez y lo inserta en su posición correcta en la matriz. Este proceso continúa hasta que se ordena la matriz.

Se utiliza un bucle anidado para el proceso de clasificación real. En cada pasada del bucle exterior for, el elemento actual se inserta en su posición correcta en la matriz.

Este proceso continúa hasta que se ordena la matriz.
Benchmark

	1.000u	10.000u	100.000u
Unsorted	1 ms
13771 ticks	104 ms
1041573 ticks	15530 ms
155305674ticks
Ascending	0 ms
64 ticks	0 ms
527 ticks	1 ms
11303 ticks
Descending	2ms
21780 ticks	212 ms
2121015ticks	33054 ms
330547989 ticks
 
Algorithm 5
Basic information
Name
SelectionSort
Complexity

	Average	Best case	Worst case
When	NA	El comportamiento tanto en el mejor de los casos como en el peor es el mismo
	El comportamiento tanto en el mejor de los casos como en el peor es el mismo
Complexity	O(n²)	O(n²)	O(n²)

References
https://www.happycoders.eu/algorithms/selection-sort/
How does it work
Selection Sort es un algoritmo de ordenación que encuentra el valor mínimo en la
matriz para cada iteración del bucle. A continuación, este valor mínimo se intercambia con el elemento de matriz actual. Este procedimiento se sigue hasta que se ordena la matriz.
Se utiliza un bucle anidado para el proceso de clasificación real. En cada pasada del
bucle for externo, se encuentra el elemento más pequeño de la matriz y se reemplaza por el elemento actual. Este proceso continúa hasta que se ordena la matriz.Benchmark

	1.000u	10.000u	100.000u
Unsorted	1 ms
14943 ticks	166 ms
1041573 ticks	18859 ms
188591127 ticks
Ascending	1 ms
14977 ticks	166 ms
1668415 ticks	18581 ms
185812353 ticks
Descending	1 ms
16825 ticks	287 ms
297 ticks	18673 ms
186739879ticks
 

Conclusion


Es más recommendable elegir el algoritmo QuickSort ya que, según se demuestra en las tablas de referencia y para los casos presentados (1.000u, 10.000u y 100.000u), los resultados en tiempos en general para practicamente todos los casos y en concreto en lo que se refiere a las formas de ordenación de Unsorted y Descending son inferiores . Por otra parte y en la comparativa con el algoritmo Insertionsort, el Ascending con el QuickSort se puede considerer en valores similares. 
