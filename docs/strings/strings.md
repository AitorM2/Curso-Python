# Aquí se van a mostrar las diferentes cosas que se pueden hacer con las strings

## Acceder a caracteres de una palabra

> En este apartado vamos a ver ejemplos de como se acceder a una letra de una palabra.

* Ejemplo para acceder a la primera letra

``` python
# Definimos la palabra
palabra = "Papel"

# Definimos la variable donde vamos a almacenar la primera letra
# y como si fuera una array le decimos que vamos a acceder a la primera posición
# en este caso le ponemos el número cero (0)
primera_letra = palabra[0]

# Mostramos por pantalla la palabra
print(palabra) # Resultado -> Papel

# Mostramos por pantalla la letra a la que hemos accedido
print(primera_letra) # Resultado -> P
```

* Ejemplo para acceder a la tercera letra

``` python
# Definimos la palabra
palabra = "Piedra"

# Definimos la variable donde vamos a almacenar la tercera letra
# y como si fuera una array le decimos que vamos a acceder a la tercera posición
# en este caso le ponemos el número dos (2)
tercera_letra = palabra[2]

# Mostramos por pantalla la palabra
print("\n" + palabra) # Resultado -> Piedra

# Mostramos por pantalla la letra a la que hemos accedido
print(tercera_letra) # Resultado -> e
```

## Dividir palabras

> En este apartado vamos a ver ejemplos de como dividir una palabra dejando los caracteres deseados.

* Ejemplo para coger las tres primeras letras

``` python
# Definimos la palabra
palabra = 'Sustraer'

# Vamos a obtener las tres primeras letras, para realizar esto lo tratamos como una array,
# le decimos que empieze en la posición cero y termine en la tres pero al decirle que termine 
# en la tres no nos va a incluir la letra que esta en la posición seis
primeras_tres = palabra[0:3]

# Mostramos la palabra completa
print(palabra)

# Mostramos por pantalla las tres primeras letras de la palabra
print(primeras_tres) # Resultado -> Sus

```

* Ejemplo para coger las tres ultimas letras

``` python

# Definimos la palabra
palabra = 'Atrapar'

# Ahora vamos a obtener las tres últimas letras, para realizar esto lo tratamos como una array,
# le decimos que empieze en la posición cuatro y termine en la siete pero al decirle que termine 
# en la siete no nos va a incluir la letra que esta en la posición siete
ultimas_tres = palabra[4:7]

# Mostramos la palabra completa
print(palabra)

# Mostramos por pantalla las ultimas tres letras de la palabra
print(ultimas_tres) # Resultado -> par
```

## Omitir caracteres de una palabra

> En este apartado vamos a ver ejemplos de como omitir caracteres de una palabra.

``` python
# Definimos la frase
frase = "Convivir"

# Definimos la variable donde vamos a almacenar la frase con caracteres omitidos
# para realizar esto tenemos que tratarlo como una array le decimos que empieze en la letra
# que se encuentra en la posición cero y que se detenga antes de llegar a la letra en la posición 7
# después le decimos que coja una letra y se salte otra de forma alternada, es decir, en este caso coge
# las letras que se encuentran en las posiciones 0, 2, 4 y 6  
frase_final = frase[0:7:2]

# Mostramos por pantalla la frase antes de realizar la omisión de letras
print(frase)

# Mostramos por pantalla el resultado 
print(frase_final) # Resultado -> Cnii
```

## Obtener longitud de una frase o de una palabra 

> En este apartado vamos a ver ejemplos de como obtener la longitud de una frase o una palabra usando el método **len()**.

* Ejemplo de explicación para obtener la longitud de una sola letra
``` python
# Definimos la letra 
letra = "A"

# Mostramos por pantalla la letra
print(letra) # Resultado -> A

# Mostramos por pantalla la longitud de la letra, para mostrar la longitud usamos
# la función predefinida que tiene python len()
print(len(letra)) # Resultado -> 1
```

* Ejemplo para obtener la longitud de una palabra
``` python
# Definimos la palabra
palabra = "Picapica"

# Mostramos por pantalla la palabra
print(palabra) # Resultado -> Picapica

# Mostramos por pantalla la longitud de la palabra, para mostrar la longitud usamos
# la función predefinida que tiene python len()
print(len(palabra)) # Resultado -> 8
```

* Ejemplo para obtener la longitud de una frase
``` python
# Definimos la frase
frase = "He comprado manzanas para merendar"

# Mostramos por pantalla la frase
print(frase) # Resultado -> He comprado manzanas para merendar

# Mostramos por pantalla la longitud de la frase, para mostrar la longitud usamos
# la función predefinida que tiene python len()
print(len(frase)) # Resultado -> 34
```

## Descomponer una palabra letra por letra

> En este apartado vamos a ver un ejemplo de como descomponer una palabra.

``` python
# Definimos el nombre de la variable y le introducimos el texto deseado
palabra = "Hola"

# Para descomponer la palabra definimos diferentes variables para cada caracter que tenga nuestra frase
# y despues le decimos que esas variables van a ser igual a la variable de la palabra
a,b,c,d = palabra

# Mostramos por pantalla la palabra sin descomponer 
print("Frase sin descomponer: " + palabra)

# Mostramos por pantalla variable por variable que hemos creado anteriormente, esto nos mostraria cada caracter
print("\nFrase descompuesta caracter por caracter: ")
print(a) # Caracter -> H
print(b) # Caracter -> O
print(c) # Caracter -> L
print(d) # Caracter -> A
```

## Concatenar palabras, letras o frases

> En este apartado vamos a ver ejemplos de como concatenar cadenas de texto.

* Ejemplo para concatenar sin espacios
``` python
# Definimos la primera palabra o frase
Nombre = "Luis"
# Definimos la segunda palabra o frase
Apellido = "Martinez"

print("Concatenación sin espacios: ")

# Mostramos por pantalla la concatenación, para concatenar palabras o frases 
# utilizamos el signo mas(+) para indicarle que queremos unir esas dos varibles
print(Nombre + Apellido) # Resultado -> LuisMartinez
```

* Ejemplo para concatenar con espacios
``` python
# Definimos la primera palabra o frase
Nombre = "Laura"
# Definimos la segunda palabra o frase
Apellido = "Gonzalez"
# Definimos el separador que queremos utilizar, es decir, le podemos dar
# cualquier nombre a la variable pero es recomendable darle un nombre significativo
# en este caso lo vamos a separar con espacios
espacio = ' '

print("\nConcatenación con espacio: ")

# Mostramos por pantalla la concatenación incluyendo el separador, es decir, la variable espacio
print(Nombre + espacio + Apellido) # Resultado -> Laura Gonzalez
```

* Ejemplo para concatenar con puntos, asteriscos, guiones, etc

``` python
# Definimos la primera palabra o frase
Nombre = "Paco"
# Definimos la segunda palabra o frase
Apellido = "Rodriguez"
# Definimos el separador que queremos utilizar, es decir, le podemos dar
# cualquier nombre a la variable pero es recomendable darle un nombre significativo
# en este caso lo vamos a separar con puntos
punto = '.'

print("\nConcatenación con punto: ")

# Mostramos por pantalla la concatenación incluyendo el separador, es decir, la variable espacio
print(Nombre + punto + Apellido) # Resultado -> Paco.Rodriguez
```

## Introducir por valores por teclado

> En este apartado vamos a ver ejemplos de como introducir valores por teclado con el método **input()**, en este ejemplo pide que introduzcamos números pero podemos cambiar ese texto y pedir lo que necesitamos.

* Caso para números

``` python
# Definimos la variable que va a almacenar el valor que vamos a introducir
numero = input("Introduce un número: ")

# Mostramos por pantalla el valor introducido
print(numero)
```

* Caso en el que queramos que introduzcan texto

``` python
# Definimos la variable que va a almacenar el valor que vamos a introducir
texto = input("Introduce una palabra: ")

# Mostramos por pantalla el valor introducido
print(texto)
```

## Métodos que se pueden usar con los strings

> En este apartado vamos a ver ejemplos de los diferentes métodos que hay y que se pueden usan.

### Método capitalize()

* Método capitalize(): Este método se usa para convertir la primera palabra de una frase a mayúsculas.

``` python
# Definimos la frase
frase1 = "el sol brilla mucho"

print("Método capitalize(): ")

# Mostramos por pantalla la frase original
print(frase1)

# Mostramos por pantalla la frase con la primera letra en mayúsculas usando el método capitalize()
print(frase1.capitalize()) # Resultado -> El sol brilla mucho
```

### Método count()

* Método count(): Este método se usa para contar cuantas veces aparece una letra en la frase.

``` python
# Definimos la frase
frase2 = "el coche aparcado es rojo"

print("\nMétodo count(): ")

# Mostramos por pantalla la frase original
print(frase2)

# Mostramos por pantalla el conteo de Oes que tiene la frase usando el método count()
print(frase2.count('o')) # Resultado -> 4
```

### Método endswith()

* Método endswith(): Este método se usa para comprobar si una frase termina con algo en específico,
este método es un boolean, es decir, si acaba de esa forma o no (true o false).

``` python
# Definimos la frase
frase3 = "los arboles son altos"

print("\nMétodo endswith(): ")

# Mostramos por pantalla la frase original
print(frase3)

# Mostramos por pantalla si esa frase acaba de la forma que le decimos o no
print(frase3.endswith("os")) # Resultado -> True
print(frase3.endswith("los")) # Resultado -> False
```
### Método expandtabs()

* Método expandtabs(): Este método se usa para reemplazar todos los caracteres de tabulación (\t)
en una frase por un número específico de espacios.

``` python
# Definimos la frase
frase4 = "Me\tvoy\tde\tvacaciones"

print("\nMétodo expandtabs(): ")

# Mostramos por pantalla la frase original
print(frase4)

# Mostramos por pantalla la frase con los espacios deseados
print(frase4.expandtabs(0)) # Resultado -> Mevoydevacaciones
print(frase4.expandtabs(20)) # Resultado -> Me                  voy                 de                  vacaciones
```
### Método find()

* Método find(): Este método se usa para buscar una palabara específica en una frase y nos devuelve 
el número en el que empieza y aparece esa palabra. Si esa palabra no se encuentra devuelve -1.

``` python
# Definimos la frase
frase5 = "Bienvenidos al curso de programacion"

print("\nMétodo find(): ")

# Mostramos por pantalla la frase original
print(frase5)

# Mostramos por pantalla el número de donde aparece por primera vez esa palabra 
# y si no existe muestra -1

print(frase5.find("curso")) # Resultado -> 15
print(frase5.find("hola")) # Resultado -> -1
```
### Método format()

* Método format(): Este método se usa para dar formato a Strings, permitiendo insertar valores
dentro de un texto utilizando marcadores de posición {}. Esta es una forma poderosa y flexible
de construir cadenas.

``` python
# Definimos las variables que vamos a usar para dar formato
nombre6 = "Pedro"
apellido6 = "Martinez"

# Definimos la frase que contiene las variables usadas para dar formato

frase6_formato = "Hola {} {}, bienvenido al sistema".format(nombre6, apellido6)

print("\nMétodo format(): ")

# Mostramos por pantalla la String con el formato
print(frase6_formato) # Resultado -> Hola Pedro Martinez, bienvenido al sistema
```
### Método index()

* Método index(): Este método es similar al método find() se usa para buscar una subcadena dentro 
dentro de una cadena y nos devuelve el índice de la primera aparición. Sin embargo, a diferencia
del método find(), si la subcadena no se encuentra, index() lanza una expcepción llamada ValueError.

``` python
# Definimos la frase
frase7 = "Aprender python es divertido"

print("\nMétodo index(): ")

# Mostramos por pantalla la frase original
print(frase7)

# Mostramos por pantalla el numero de veces que aparece una letra o conjunto de letras y  
# si no lo encuentra nos muestra el error ValueError
print(frase7.index("e")) # Resultado -> 3
```

### Método isalnum()

* Método isalnum(): Este método se usa para verificar si todos los caracteres de una cadena son
alfanuméricos, es decir, si son letras (a-z, A-Z) o son número (0-9).

``` python
# Definimos la frase sin espacios
frase8 = "TreintaDiasDePython"

# Definimos la frase con espacios
frase81 = "Ejemplos de Python"

print("\nMétodo isalnum(): ")

# Mostramos por pantalla las frases originales
print(frase8)
print(frase81)

# Mostramos por pantalla si la cadena contiene valores alfanuméricos mostrandonos true y 
# en caso de que contenga espacios nos motrará false ya que los espacios no son alfanuméricos
print(frase8.isalnum()) # Resultado -> true
print(frase81.isalnum()) # Resultado -> false
```

### Método isalpha()

* Método isalpha(): Este método se usa para verificar si todos los caracteres de una cadena son
alfabéticos, es decir, si son letras (a-z, A-Z).

``` python
# Definimos la frase sin numeros
frase9 = "Vivoenunchalet"

# Definimos la frase con numeros
frase91= "Elnumeroesel29"

print("\nMétodo isalpha(): ")

# Mostramos por pantalla las frases originales
print(frase9)
print(frase91)

# Mostramos por pantalla si la cadena contiene valores alfabéticos mostrandonos true y 
# en caso de que contenga números nos motrará false ya que los número no son alfabéticos
# otro caso que nos puede mostrar false es una frase con espacios, ya que los espacios
# no son alfabéticos
print(frase9.isalpha()) # Resultado -> true
print(frase91.isalpha()) # Resultado -> false
```
### Método isdecimal()

* Método isdecimal(): Este método se usa para verificar si todos los caracteres de una cadena son
número decimales, esto significa que la cadena solo puede contener número enteros sin decimales
sin signos negativos, ni otros caracteres no númericos.

``` python
# Definimos la frase con números decimales
frase10 = "1234"

# Definimos la frase sin numeros decimales
frase101= "-5678"

print("\nMétodo isdecimal(): ")

# Mostramos por pantalla las frases originales
print(frase10)
print(frase101)

# Mostramos por pantalla si la cadena contiene valores decimales mostrandonos true y 
# en caso de que contenga dígitos no decimales nos motrará false ya que como se ha mencionado
# anteriormente si contiene signo negativo u otros caracteres nos mostrará false
print(frase10.isdecimal()) # Resultado -> true
print(frase101.isdecimal()) # Resultado -> false
```

### Método isdigit()

* Método isdigit(): Este método es un método incorporado que se usa para verificar si todos 
los caracteres de una cadena está formada únicamente por números, sin embargo, isdigit()
es más amplio que isdecimal(), ya que también acepta otros tipos de dígitos numéricos que 
no sean solo número del 0-9, como los números en otros sistemas numéricos
(como por ejemplo, números romanos o dígitos de otros alfabetos).

``` python
# Definimos la frase con números decimales
frase11 = "1234"

# Definimos la frase sin numeros decimales
frase111= "567.8"

print("\nMétodo isdigit(): ")

# Mostramos por pantalla las frases originales
print(frase11)
print(frase111)

# Mostramos por pantalla si la cadena contiene valores decimales mostrandonos true y 
# en caso de que contenga dígitos no decimales nos motrará false ya que como se ha mencionado
# anteriormente si contiene signo negativo u otros caracteres nos mostrará false
print(frase11.isdigit()) # Resultado -> true
print(frase111.isdigit()) # Resultado -> false
```
### Método isidentifier()

* Método isidentifier(): Este método se usa para comprobar si una cadena es un 
identificador válido en Pyhton. Un identificador es una secuencia de caracteres 
que puede ser utilizada como nombre para variables, funciones, clases, etc.

Para que una cadena sea un identificador válido en Python, debe seguir estas reglas:

- Solo puede contener letras (Mayúsculas o minusculas), digitos (0-9) y guiones bajos ( _ ).
- No puede comenzar con un número.
- No puede ser una palabra reservada como (if, for, while, etc).

``` python
print("\nMétodo isidentifier(): ")

# Mostramos por pantalla si los siguientes nombres de variables son identificadores válidos

print("variable1".isidentifier()) # Resultado -> true
print("1variable".isidentifier()) # Resultado -> false | Ya que comienza con un número (Regla 2)
print("mi_variable".isidentifier()) # Resultado -> true 
```

### Método islower()

* Método islower(): Este método se usa para comprobar si todas las letras de una cadena de texto son minúsculas.

``` python
# Definimos la frase en minusculas
frase13 = "hola"

# Definimos la frase con una letra en mayusculas
frase131 = "Prueba"

print("\nMétodo islower(): ")

# Mostramos por pantalla las frases originales
print(frase13)
print(frase131)

# Mostramos por pantalla si las siguientes cadenas estan en minusculas o no, si estan en minusculas nos 
# devolverá true en caso contrario nos mostrará false

print(frase13.islower()) # Resultado -> true
print(frase131.islower()) # Resultado -> false
```

### Método isupper()

* Método isupper(): Este método se usa para comprobar si todas las letras de una cadena de texto son mayúsculas.

``` python
# Definimos la frase en minusculas
frase14 = "COCHE"

# Definimos la frase con una letra en mayusculas
frase141 = "moto"

print("\nMétodo isupper(): ")

# Mostramos por pantalla las frases originales
print(frase14)
print(frase141)

# Mostramos por pantalla si las siguientes cadenas estan en mayusculas o no, si estan en mayusculas nos 
# devolverá true en caso contrario nos mostrará false

print(frase14.isupper()) # Resultado -> true
print(frase141.isupper()) # Resultado -> false
```

### Método isnumeric()

* Método isnumeric(): Este método se usa para comprobar si toda la cadena consiste en números, es decir, 
que la frase debe contener solo números y no puede contener letras, espacios o símbolos.

``` python
# Definimos la frase con numeros
frase15 = "123"

# Definimos la frase con numeros y letras
frase151 = "456abc"

print("\nMétodo isnumeric(): ")

# Mostramos por pantalla las frases originales
print(frase15)
print(frase151)

# Mostramos por pantalla si las siguientes cadenas estan formadas solo por numeros o no, 
# si estan formada solo por números nos devolverá true en caso contrario nos mostrará false

print(frase15.isnumeric()) # Resultado -> true
print(frase151.isnumeric()) # Resultado -> false
```

### Método join()

* Método join(): Este método se usa para unir una secuencia ya sea una lista, tupla o cualquier otro itinerable
de cadena de texto en una sola cadena. Este método coge como argumento un itinerable que contiene cadenas y 
la concatena, usando el string que lo llama como separador.

``` python
# Definimos la sentencia
frase16 = ["peras", "uvas", "sandias"]

# Definimos el resultado separado con espacios
frase161 = " ".join(frase16)

# Definimos el resultado separado con guiones
frase162 = "-".join(frase16)

print("\nMétodo join(): ")

# Mostramos por pantalla la sentencia
print(frase16)

# Mostramos por pantalla los resultados concatenados
print(frase161) # Resultado -> peras uvas sandias
print(frase162) # Resultado -> peras-uvas-sandias
```

### Método strip()

* Método strip(): Este método se usa para eliminar los espacios en blanco o caracteres especificados
al principio o al final de una cadena de texto. No elimina los caracteres del medio de la cadena,
solo elimina los del principio y los del final.

``` python
# Definimos la frase con espacios en blanco
frase17 = " Hola, que tal? "

print("\nMétodo strip(): ")

# Mostramos por pantalla las frases originales
print(frase17)

# Mostramos por pantalla los resultados usando el método strip()
print(frase17.strip()) # Resultado -> Hola, que tal?
```
### Método replace()

* Método replace(): Este método se usa para reemplazar una subcadena específica en una cadena por
otra subcadena. Este método no modifica la cadena original, sino que devuelve una nueva con las
situaciones realizadas.

``` python
# Definimos la frase
frase18 = "Estoy aprendiendo java"

print("\nMétodo replace(): ")

# Mostramos por pantalla la frase original
print(frase18)

# Mostramos por pantalla la frase reemplazando java por python
print(frase18.replace('java', 'python')) # Resultado -> Estoy aprendiendo python
```

### Método split()

* Método split(): Este método se usa para dividir una cadena en una lista de subcadenas, utilizando un
delimitador específico como un espacio, una coma, etc. Si no se especifica un delimitador, divide
la cadena en cada espacio en blanco.

``` python
# Definimos la frase con division por espacios
frase19 = "Bienvenido a Python"

print("\nMétodo split(): ")

# Mostramos por pantalla la frase original
print(frase19)

# Mostramos por pantalla la frase dividida
print(frase19.split()) # Resultado -> ['Bienvenido', 'a', 'Python']
```
### Método title()

* Método title(): Este método se usa para devolver una cadena donde la primera letra de cada palabra
esta en mayuscula y el resto de las letras estan en minuscula. Este método es util para formatear
titulos o nombres de manera consistente.


``` python
# Definimos la frase
frase20 = "mi casa es blanca"

print("\nMétodo title(): ")

# Mostramos por pantalla la frase original
print(frase20)

# Mostramos por pantalla la frase modificando las primeras letras
print(frase20.title()) # Resultado -> Mi Casa Es Blanca
```
### Método swapcase()

* Método swapcase(): Este método se usa para devolver una nueva cadena donde las letras en mayusculas
se convierten en minuscula y las letras en minuscula se convierten en mayuscula. Este método es 
util para invertir rapidamente el caso de los caracteres en una cadena.

``` python
# Definimos la frase
frase21 = "Fruteria Paco"

print("\nMétodo swapcase(): ")

# Mostramos por pantalla la frase original
print(frase21)

# Mostramos por pantalla la frase modificando las mayusculas y las minusculas
print(frase21.swapcase()) # Resultado -> Fruteria Paco
```
### Método startswith()

* Método startswith(): Este método se usa para verificar si una cadena comienza con una subcadena específica
devuelve un valor booleano true si la cadena comienza con la subcadena especificada
o false si no comienza con la subcadena.

``` python
# Definimos la frase
frase22 = "Que te calles"
frase221 = "Esto es un chorizo"

print("\nMétodo startswith(): ")

# Mostramos por pantalla las frases originales
print(frase22)
print(frase221)

# Mostramos por pantalla las frases mostrando si tienen ese comienzo o no
print(frase22.startswith("Que")) # Resultado -> true 
print(frase221.startswith("chorizo")) # Resultado -> false
```