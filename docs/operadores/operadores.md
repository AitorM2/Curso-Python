# Aquí se van a mostrar los diferentes tipos de operadores que hay en python y su uso

> Los operadores que hay son iguales que en otros lenguajes de programación con la unica peculiaridad y es que en este caso
para definir un numero con exponente no necesitamos usar nada como en java.

## Operadores de cálculo

* Ejemplo de operador de suma

```python
suma = 4 + 1
```

* Ejemplo de operador de resta

```python
resta = 3 - 1
```

* Ejemplo de operador de multiplicación

```python
multiplicacion = 6 * 2
```

* Ejemplo de operador de división

```python
division = 20 / 3
```

* Ejemplo de operador de división sin resto

```python
divisionsinresto = 20 // 3
```

* Ejemplo de operador de módulo, este tipo nos entrega el resto de una división

```python
modulo = 3 % 2
```

* Ejemplo de operador de exponente, es decir, un número elevado a x

```python
exponente = 3 ** 2
```

### Comprobación del resultado de cada variable de cálculo

``` python
print(suma) # Resultado -> 5
print(resta) # Resultado -> 2
print(multiplicacion) # Resultado -> 12
print(division) # Resultado -> 6.666666666666667
print(divisionsinresto) # Resultado -> 6
print(modulo) # Resultado -> 1
print(exponente) # Resultado -> 9 
```

## Operadores de comparación

* Ejemplo de operador de mayor que

```python
mayor = 5 > 3
```

* Ejemplo de operador de menor que

```python
menor = 10 < 9
```

* Ejemplo de operador de mayor o igual que

```python
mayoroigual = 1 >= 3
```

* Ejemplo de operador de menor o igual que

```python
menoroigual = 12 <= 44
```

* Ejemplo de operador de igual a que

```python
igual = 8 == 8
```

* Ejemplo de operador de diferente de que

```python
diferente = 15 != 15
```

### Comprobación del resultado de cada variable de comparación

``` python
print(mayor) # Resultado -> True 
print(menor) # Resultado -> False
print(mayoroigual) # Resultado -> False
print(menoroigual) # Resultado -> True
print(igual) # Resultado -> True
print(diferente) # Resultado -> False
```
> En este caso nos va a mostrar False ya que en la variable le hemos preguntado si 15 es diferente de 15,
por eso nos dice False. Si le pasaramos dos números diferentes nos diria True.
``` python
diferente = 15 != 15
print(diferente) # Resultado -> False
```

## Definicion de las variables de comparación usando palabras reservadas

* Ejemplo de operador de igual a algo usando palabra reservada

```python
igual2 = 2 is 2
```

* Ejemplo de operador de no es algo usando palabra reservada

```python
noes = 3 is not 2
```

* Ejemplo de operador de comprobar si una palabra contiene una letra

```python
contiene = 'A' in 'Avión'
```

* Ejemplo de si contiene varias letras

```python
contiene2 = 'es' in 'Mi coche es rojo'
```

### Comprobación del resultado de cada variable de comparación con palabras reservadas

``` python
print(igual2) # Resultado -> True
print(noes) # Resultado -> True
print(contiene) # Resultado -> True
print(contiene2) # Resultado -> True
```