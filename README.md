#Reto 4

#numeros primos



 pseudocodigo



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
    # Inicializamos los valores de a, b y epsilon
    a = 0
    b = numero
    c = 0.00001

    # Mientras la diferencia entre a y b sea mayor que epsilon
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