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

Diagrama de flujo


 [![a.png](https://i.postimg.cc/N0F9H5vr/a.png)](https://postimg.cc/xkr1rjC0)

 pseudocodigo


````python
# Inicialización de variables
num = float(input("ingresa un numero"))
a = 0
b = num
c = 0.00001  # Margen de error 

# Algoritmo de aproximación por división y resta
while True:
    promedio = (a + b) / 2.0
    if abs(promedio**2 - num) <= c:
        break
    elif promedio**2 < num:
        a = promedio
    else:
        b = promedio

# Imprimimos el resultado
print("La raíz cuadrada de", num, "es:", promedio)

````
