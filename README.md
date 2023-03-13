#Reto 4

#numeros primos

Diagrama de flujo

[![Captura.png](https://i.postimg.cc/tRnK5SmJ/Captura.png)](https://postimg.cc/QVsYNbDZ)

 pseudocodigo

```python
n = int(2) #establecemos el divisor y dividendo como enteros
i = int(2) 

while n < 1000: #mientras el valor del dividendo sea menor a mil
    if n == 2: #si el dividendo es igual a dos es primo
        print(n, "es primo")
    if n%i == 0: #si el numero es divisible por residuo y da cero 
        n = n+1 #se aumenta el numero dividendo en uno
        i = 2 #se restable el valor de el divisor a dos
    else: 
        i = i+1 #sino el divisor se aumenta en uno 
        if i == n-1: #se el dividor es menor que el dividendo en uno es primo
            print(n, "es primo")
```

#Raiz cuadrada

```python
Inicio
Leer el número al que se le va a calcular la raíz cuadrada (numero)
Inicializar a = 0
Inicializar b = numero
Inicializar c = 0.00001
Mientras abs(a - b) > c, hacer lo siguiente:
    Calcular el punto medio x = (a + b) / 2.0
    Si x*x > numero, entonces:
        b = x
    De lo contrario:
        a = x
Devolver x como la raíz cuadrada de numero
Fin
```

 pseudocodigo


````python
def calcular_raiz_cuadrada(numero):
    # Inicializamos los valores de a, b y c
    a = 0
    b = numero
    c = 0.00001

    # Mientras la diferencia entre a y b sea mayor que c
    while abs(a - b) > c:
        # Calculamos el punto medio de a y b
        x = (a + b) / 2.0
        # Si x al cuadrado es mayor que el número, nos movemos hacia la izquierda
        if x*x > numero:
            b = x
        # Si x al cuadrado es menor que el número, nos movemos hacia la derecha
        else:
            a = x

    # Devolvemos el valor de x, que es la raíz cuadrada aproximada del número
    return x

````
