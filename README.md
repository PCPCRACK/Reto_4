# Reto_4



#Raiz pseudocodigo




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
