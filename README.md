# Reto_4
#numeros primos





 pseudocodigo



#Raiz cuadrada

inicio
Ingresa el número cuya raíz cuadrada deseas obtener
Divide el número en grupos de dos dígitos, comenzando por la derecha
Si el número de dígitos es impar, añade un cero al final
Coloca un punto sobre el último dígito del grupo de la izquierda, y otro punto debajo del mismo dígito
Encuentra el número más grande cuyo cuadrado sea menor o igual al número del grupo de la izquierda
Escribe ese número en la parte superior del punto
Resta el cuadrado de ese número del grupo de la izquierda, y lleva el resultado al siguiente grupo
Baja el siguiente grupo y añade el resultado de la resta anterior
Divide el número en la parte superior del punto por dos y escribe el resultado debajo del grupo bajado
Multiplica el número en la parte superior del punto por el número que acabas de escribir, y coloca el resultado debajo del grupo bajado
Resta el número que acabas de escribir debajo del grupo bajado, y lleva el resultado al siguiente grupo
Si has terminado de bajar grupos, tu resultado es la parte superior del punto seguida de los números debajo del punto
Si aún te quedan grupos por bajar, regresa al paso 6


 pseudocodigo


````python
Inicio
|
|___ Leer el número del cual se desea calcular la raíz cuadrada
|
|___ Si el número es cero, retornar cero
|       |
|       |___ Fin
|
|___ Calcular la potencia de 2 más cercana al número de entrada
|       |
|       |___ Dividir el número por dos y calcular su logaritmo en base 2
|       |
|       |___ Calcular la potencia de 2 del resultado anterior
|       |
|       |___ Si el número original es menor que la potencia de 2 calculada,
|             restar 1 a la potencia de 2
|
|___ Inicializar la variable x como la potencia de 2 calculada
|
|___ Mientras se cumpla la condición de salida
|       |
|       |___ Calcular la variable y como el promedio entre x y el cociente
|             de la división del número por x
|       |
|       |___ Si y es mayor o igual que x, retornar x
|       |
|       |___ Asignar y a x
|
|___ Fin
````