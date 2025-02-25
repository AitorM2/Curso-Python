# Aquí se va a mostrar como definir una función y que es una función

> Una función es un bloque de código que sólo se ejecuta cuando se llama, puede pasar datos conocidos como parámetros, a una función y además una función puede devolver datos como resultado.

## Creación de una función

> En Python una función se define usando la palabra clave **def:**

* Ejemplo de una función básica

``` python
def my_function():
  print("Hola desde una función")
```

* Ejemplo de como llamar a una función

``` python
def my_function():
  print("Hola desde una función")

my_function()
```

> Al ejecutar este ejemplo nos dará este resultado: 

``` cmd
Hola desde una función
```
> Ya que al usar `my_function()` estariamos llamando a la función para que se ejecute.

## Pasar argumentos a una función

> La información se puede pasar a las funciones como argumentos. Los argumentos se especifican después del nombre de la función, dentro del paréntesis. Puedes agregar tantos argumentos como quieras, simplemente sepáralos con una coma.


* En el siguiente ejemplo tienes una función con un argumento (fname). Cuando se llama a la función, pasamos un nombre, que se usa dentro de la función para imprimir el nombre completo:

``` python
def my_function(fname):
  print(fname + " Martinez")

my_function("Luis")
my_function("Paco")
my_function("Laura")
```

> Resultado de ejecutar la función anterior:

``` cmd
Luis Martinez
Paco Martinez
Laura Martinez
```


## Números de argumentos

> De forma predeterminada, se debe llamar a una función con la cantidad correcta de argumentos. Lo que significa que si tu función espera 2 argumentos, debes llamar a la función con 2 argumentos, ni uno más ni uno menos.

* Ejemplo de una función que espera 2 argumentos y le pasamos dos argumentos.

``` python
def my_function(fname, lname):
  print(fname + " " + lname)

my_function("Sergio", "Gonzalez")
```

> Resultado de ejecutar la función anterior:

``` cmd
Sergio Gonzalez
```

> Si intentamos llamar a la función con 1 o 3 argumentos, obtendrás un error.

* Ejemplo de una función que espera dos argumentos y le pasamos 1.

``` python
def my_function(fname, lname):
  print(fname + " " + lname)

my_function("Sergio")
```

> Resultado de ejecutar la función anterior:

``` cmd
my_function("Sergio")
    ~~~~~~~~~~~^^^^^^^^^^
TypeError: my_function() missing 1 required positional argument: 'lname'
```