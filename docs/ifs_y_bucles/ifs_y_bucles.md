# Aquí se van a mostrar como realizar un IF y los dos tipos de bucles que hay

> Para realizar una comparación usando if's se define de forma distinta a java

## Uso y definición de un if

* Este es un ejemplo de un ejercicio básico paso a paso del uso de un if para comprobar si un numero es mayor a otro o viceversa.

``` python
# Definimos las variables que vamos a comparar
a = 5
b = 10

# Realizamos la comparación y mostramos por pantalla el resultado
if a > b:
    print(a, " es mayor que ", b) # En este caso si a es mayor a b, nos motrará el mesaje 1
else:
    print(a, " es menor que ", b) # En este caso si a es menor que b, nos motrará el mensaje 2
```

**Mensaje 1**
``` cmd
20  es mayor que  10
```

**Mensaje 2**
``` cmd
 5 es menor que  10
```

* Este es un ejemplo de un ejercicio mas complejo paso a paso del uso de un if para comprobar introduciendo la edad por pantalla si eres mayor de edad o no.

``` python

# Definimos la variable que va a recibir el valor introducido por teclado, pero 
# no podemos comparar string con numeros entonces le decimos que lo que le vamos 
# a introducir por teclado es un entero usando el metodo que tiene python que es int()

edad = int(input("Introduce la edad: "))

if edad >= 18:
    print("Eres mayor de edad")
else:
    print("Eres menor de edad")
```

## Tipos de bucles

### Bucle for

> Para realizar el bucle for usaremos la siguiente estructura.

* Ejemplo para mostrar todas las frutas que tiene una array usando un bucle for.

``` python
frutas = ['peras', 'platanos', 'manzanas', 'naranjas']

for x in frutas:
    print(x)
```

> Resultado del ejemplo:

``` cmd
peras
platanos
manzanas
naranjas
```

* Ejemplo para mostrar como el bucle for separa una por una las letras que tiene una palabra.
``` python
palabra = "Aparcamiento"

for x in palabra:
    print(x)
```
> Resultado del ejemplo:

``` cmd
A
p
a
r
c
a
m
i
e
n
t
o
```

### Bucle while

> Para realizar un bucle while realizaremos la siguiente estructura

* Ejemplo para ver como aumenta el contador.

``` python
# Definimos el contador
i = 1

# Realizamos el bucle while mostrando como aumenta el contador
while i < 6:
    print(i)
    i += 1
```

> Resultado del ejemplo:

``` cmd
1
2
3
4
5
```

* Ejemplo para ver como aumenta el contador pero haciendo que se pare en un número en concreto.

``` python
# Definimos el contador
k = 1

# Realizamos el bucle while mostrando como aumenta el contador, 
# pero diciendole que cuando sea 7 que detenga el programa
while k < 9:
    print(k)
    if k == 7:
        break
    k += 1
```

> Resultado del ejemplo:

``` cmd
1
2
3
4
5
6
7
```