# Funciones y variables. 

## Archivos en Python.
Todos los programas que se escriben en lenguaje Python se deben guardar en un archivo con extención .py con la finalidad de indicarle a la computadora que efectivamente estamos trabajando en un programa de Python.

```python
nombre_archivo.py
```

Para ejecutar el programa debemos utilizar la siguiente sintaxis en la terminal o consola de comando:

```python
python nombre_archivo.py
```

## Comentarios en Python.
Los **comentarios** en Python *son fragmentos de texto que no se ejecutan como código*. Se utilizan para explicar el código, documentar el funcionamiento del programa o simplemente para hacer anotaciones.  

Hay dos tipos de comentarios en Python:  

* **Comentarios de línea única**: Se inician con el símbolo numeral (#) y se extienden hasta el final de la línea.  

* **Comentarios de bloque**: Se inician con tres comillas dobles (""") y se cierran con tres comillas dobles ("""). Pueden ocupar varias líneas.

Ejemplos de comentarios en Python:  

```python
# Este es un comentario de línea única.

"""
Este es un comentario de bloque
que ocupa varias líneas.
"""
```

Los comentarios en Python ofrecen una serie de ventajas, entre las que se incluyen:  

* **Mejor legibilidad del código**: los comentarios ayudan a que el código sea más fácil de leer y comprender.  

* **Documentación del código**: los comentarios pueden utilizarse para documentar el funcionamiento del programa, lo que facilita su mantenimiento y actualización.
  
* **Explicación del código**: los comentarios pueden utilizarse para explicar el código, lo que puede ser útil para otros programadores o para el propio programador en el futuro.

Consejos para escribir comentarios en Python:  

* **Utilice comentarios descriptivos**: los comentarios deben ser claros y concisos, y deben explicar claramente el propósito del código.
  
* **Evite los comentarios redundantes**: si el código es claro y bien escrito, no es necesario añadir comentarios redundantes.  

* **Actualice los comentarios**: si el código se modifica, asegúrese de actualizar los comentarios para que sigan siendo precisos.  

## Funciones incorporadas en Python.
Python incluye una gran cantidad de funciones incorporadas que se pueden utilizar sin necesidad de definirlas. Su sintaxis es la siguiente:  

```python
nombre_funcion_python(argumento)
```

Los *argumentos* son una entrada a una función que de alguna manera influye en su comportamiento. En la mayoria de las ocaciones los argumentos deben ir encerrados entre comillas.

```python
nombre_funcion_python("argumento")
```

### **Función print()**.
Es una función incorporada que *se utiliza para mostrar mensajes en la pantalla*. Es muy útil cuando se desea mostrar el resultado de una operación o simplemente para imprimir un mensaje para el usuario. La sintaxis básica de la función ***print()*** es la siguiente:  

```python
print(objeto)
```

Los objetos pueden ser de cualquier tipo, incluyendo cadenas de texto, números, listas, diccionarios, etc. Por ejemplo, el siguiente código imprime la cadena de texto *Hola, mundo* en la pantalla: 

```python
print("Hola, mundo")
```
Sol: Hola, mundo  

También, podemos imprimir por pantalla un mensaje que contenga más de un objeto, en este caso, cadenas de texto separados por comas "**,**".

```python
print("Hola", "mundo")    # La coma , genera un espacio entre las cadenas de texto.
```
Sol: Hola, mundo  

La función ***print()*** también tiene algunos parámetros opcionales que se pueden utilizar para personalizar la salida. Escrita en su forma general:

```python
print(*objects, sep=' ', end='\n', file=None, flush=False)
```

1. ***objects***: el objeto que se desea imprimir. Puede ser una cadena de texto, un número, una lista, una tupla, un diccionario, etc.

2. ***sep***: se utiliza para especificar el separador entre los elementos que se imprimen. El valor predeterminado de *sep* es un espacio en blanco.

3. ***end***: especificar el carácter que se utilizará al final de la salida.  

Trabajemos un poco con el parámetro ***sep*** dentro de la función ***print()*** con los siguientes ejemplos:

```python
print("Hola", "mundo", sep="...")

print("Hola", "mundo", sep="-")

print("Hola", "mundo", sep="|")

print("Hola", "mundo", sep="_")

print("Hola", "mundo", sep="/")
```
Sol:  
Hola...mundo  
Hola-mundo  
Hola|mundo  
Hola_mundo  
Hola/mundo  

Trabajemos ahora un poco con el parámetro ***end*** dentro de la función print() con los siguientes ejemplos:
```python
print("Hola", "mundo", end=".")
```
Sol: Hola mundo.  

```python
print("Hola", "mundo", end="...")
```
Sol: Hola mundo...  

```python
print("Hola", "mundo", end="!")
```
Sol: Hola mundo!  

```python
print("Hola", "mundo", end="|")
```
Sol: Hola mundo|  

Al no utilizar como argumento ***\n*** dentro del parámetro ***end*** se elimina el salto de línea (que se encuentra por defecto) al ejecutar la función ***print()***.  

### **Función input()**.
Se utiliza para solicitar al usuario que *introduzca datos por teclado*. La función ***input()** devuelve una cadena de texto*. Su sintaxis es la siguiente:

```python
input(prompt)
```

El ***prompt*** es una cadena de texto que se muestra al usuario para solicitar la entrada.

```python
input("Cual es tu nombre: ")
```
Sol:  
Cual es tu nombre:   

El usuario puede escribir su nombre en la pantalla y pulsar la tecla Enter. La función ***input()*** devolverá una cadena con el nombre del usuario. También se puede utilizar para obtener la entrada de números. Sin embargo, de forma predeterminada, la función ***input()*** convierte la entrada en un dato tipo ***string*** (cadena de texto), incluso si el usuario escribe un número. Es una herramienta muy útil para interactuar con el usuario. Se puede utilizar para obtener la entrada del usuario para cualquier propósito.  

También, podemos combinar las funciones de entrada y salida de datos:

```python
print("Hola", input("Cual es tu nombre? "))
```
Sol:  
Cual es tu nombre? *Jairo*  
Hola *Jairo*  

Más adelante estudiaremos otras funciones incorporadas en el lenguaje de Python.  

## Variables.
En Python, las *variables son nombres que se utilizan para almacenar valores en la memoria del ordenador*. Permiten guardar información para utilizarla posteriormente en el código.  

Características principales de las variables en Python:

* **No es necesario declararlas**: a diferencia de otros lenguajes, *en Python no se necesita declarar el tipo de dato de una variable* antes de usarla. El tipo se asigna automáticamente cuando se le asigna un valor por primera vez.
  
* **Tipado dinámico**: significa que el *tipo de dato de una variable puede cambiar* a lo largo del programa.
  
* **Nombres significativos**: es recomendable *utilizar nombres descriptivos para las variables*, que indiquen claramente qué tipo de información almacenan.
  
* **Sensibilidad a mayúsculas y minúsculas**: Python distingue entre mayúsculas y minúsculas en los nombres de las variables. Por ejemplo, nombre y NOMBRE son variables diferentes.  

Para crear una variable en Python, simplemente se le asigna un valor utilizando el operador de **asignación =**. Su sintaxis es la siguiente:  
```python
variable = valor
```

Python nos ofrece la posibilidad de hacer una asignación múltiple de la siguiente manera:

```python
tres = three = drei = 3

print(tres)
print(three)
print(drei)
```
Sol:  
3  
3  
3  

En este caso las tres variables utilizadas en el «lado izquierdo» tomarán el valor 3. Las asignaciones que hemos hecho hasta ahora han sido de un *valor literal* a una variable. Pero nada impide que podamos hacer asignaciones de una variable a otra variable:

```python
personas = 157432
total_personas = personas
print(total_personas)
```
Sol: 157432  

La variable que utilicemos como valor de asignación debe existir previamente, ya que si no es así, obtendremos un error informando de que no está definida.

### Reglas para nombrar variables.
En Python existen una serie de reglas para los nombres de variables:

* Sólo pueden contener los siguientes caracteres:
  * Letras minúsculas.  
  * Letras mayúsculas.  
  * Dígitos.  
  * Guiones bajos (_).  

* Deben empezar con una letra o un guión bajo, nunca con un dígito.

No se puede utilizar una palabra reservada («keywords») del lenguaje python (revisar documentación) como nombre de variable.

```python
# Programa que genera un saludo.
# Preguntar al usuario su nombre, guardar la información en una variable.
nombre = input("Cual es tu nombre: ")

# Imprimir en la consola un saludo con el nombre del usuario.
print("Hola,", nombre)
```
Sol: Cual es tu nombre: *NicLau*  
       Hola, *NicLau*  

Existe una convención para la *nomenclatura de las variables*, se utiliza el llamado **snake_case** en el que utilizamos caracteres en minúsculas (incluyendo dígitos si procede) junto con guiones bajos _ cuando sean necesarios para su legibilidad. Por ejemplo, para nombrar una variable que almacene el número de canciones en nuestro ordenador, podríamos usar num_songs.  

Un caso especial y que vale la pena destacar son las ***constantes***. Podríamos decir que es un tipo de variable pero que su valor no cambia a lo largo de nuestro programa. Por ejemplo la velocidad de la luz. Sabemos que su valor es constante de 300.000 km/s. En el caso de las constantes utilizamos mayúsculas (incluyendo guiones bajos si es necesario) para nombrarlas. Para la velocidad de la luz nuestra constante se podría llamar: LIGHT_SPEED.

También, podemos documentarnos sobre los parámetros y argumentos que se pueden aplicar a las variables, para esto podemos consultar la página oficial [docs.Python.org](https://docs.python.org/3/)

```python
# Generar un saludo con el nombre de un usuario.
# Preguntar al usuario su nombre, almacenar la información en una variable.
nombre = input("Cual es tu nombre: ")

# Utilizar un parámetro.
# .capitalize(), retorna una copia de la cadena con el primer carácter en mayúsculas y el resto en minúsculas.
nombre = nombre.capitalize()

# Imprimir en la consola un saludo con el nombre del usuario.
print("Hola,", nombre)
```
Sol: Cual es tu nombre: *nicLau*  
    Hola, *NicLau*  

También, podemos combinar parámetros:  

```python
# Generar un saludo.
# Preguntar al usuario su nombre, guardar la información en una variable.
nombre = input("Cual es tu nombre: ")

# .strip(), retorna una copia de la cadena con los caracteres indicados eliminados.
# .capitalize(), retorna una copia de la cadena con el primer carácter en mayúsculas y el resto en minúsculas.
nombre = nombre.strip().capitalize()

# Imprimir en la consola un saludo con el nombre del usuario.
print("Hola,", nombre)
```
Sol: Cual es tu nombre: (espacio en blanco) *niclau*     
Hola, *Niclau*  

```python
# Definimos una variable que contiene la información obtenida por parte del usuario.
nombre = input("Introduce tu nombre en letra mayúscula: ")

# .lower(), retorna una copia de la cadena de caracteres con todas las letras en minúsculas.
nombre_formateado = nombre.lower()

# Salida.
print(nombre_formateado)
```
Sol:
Introduce tu nombre en letra mayúscula: *MATIAS*  
matias  

```python
# Eliminar caracteres.
texto = 'www.sitio_web.comzx'
# .strip(), retorna una copia de la cadena con los caracteres indicados eliminados.
texto_trnsf = texto.strip('zx')
print(texto_trnsf)
```
Sol: www.sitio_web.com  

También, podemos utilizar estas funciones que trabajan con cadenas de textos dentro de la función ***print()***.

```python
# .upper(), convierte un string en mayúsculas.
print("Hola NicLau".upper())
```
Sol: HOLA NICLAU  

```python
# .replace(), retorna una copia de la cadena con todas las ocurrencias de la cadena antiguas sustituidas por nuevas.
print("Hola NicLau".replace(" ", "_"))
```
Sol: Hola_NicLau  

Existen muchos más métodos que estudiar en la documentación de Python por revisar.

### Como regla general.

* Usar ***nombres*** para variables (ejemplo article).  

* Usar ***verbos*** para funciones (ejemplo get_article()).  

* Usar ***adjetivos*** para booleanos (ejemplo available).

Se debe destacar que las variables son nombres, no lugares. Detrás de esta frase se esconde la reflexión de que cuando asignamos un valor a una variable, lo que realmente está ocurriendo es que *se hace apuntar el nombre de la variable a una zona de memoria en el que se representa el objeto (con su valor)*.

```python
a = 7
```

Si ahora copiamos el valor de **a** en otra variable **b** se podría esperar que hubiera otro espacio en memoria para dicho valor, pero como ya hemos dicho, son referencias a memoria.

```python
b = a
```

La función **id()** nos permite *conocer la dirección de memoria de un objeto* en Python. A través de ella podemos comprobar que las dos variables que hemos creado apuntan a la misma zona de memoria.

```python
# Asignamos un valor a la variable a.
a = 7
# Creamos una variable b que contenga a la variable a.
b = a

# Imprimirá como salida la dirección donde se almacena en la memoria los valores de las variables, en este caso debe ser la misma.
print(id(a))
print(id(b))
```
Sol:  
140353359179912  
140353359179912  

La prueba de que la zona de memoria no la ocupa el nombre de la variable, es que podemos ver cómo se asigna una dirección de memoria únicamente al valor literal.

```python
# Asignamos un valor a la variable a.
a = 7
# Creamos una variable b que contenga a la variable a.
b = 8

# Imprimirá como salida la dirección donde se almacena en la memoria los valores de las variables, en este caso debe ser diferente.
print(id(a))
print(id(b))
```
Sol:  
140614580433032  
140614580433064  

Cada vez que asignamos un nuevo valor a una variable, ésta apunta a una nueva zona de memoria. Cuando la zona de memoria que ocupa el objeto se puede modificar hablamos de tipos de datos mutables. En otro caso hablamos de tipos de datos inmutables.  

## Concatenación en Python.
Es el proceso de *unir dos o más cadenas de texto*. Se puede realizar utilizando el operador de concatenación **+**.  

Sintaxis de la concatenación en Python:  

```python
cadena1 = "texto1, "
cadena2 = "texto2"

print(cadena1 + cadena2)
```
Sol: texto1, texto2  

Otras formas de concatenar cadenas en Python:  
* **Método format()**: se puede utilizar para concatenar cadenas de texto y valores.

```python
nombre = "NicLau"
edad = 15

print("Hola, mi nombre es {} y tengo {} años.".format(nombre, edad))
```
Sol: Hola, mi nombre es *NicLau* y tengo *15* años.  

* **Operador f-string**: se puede utilizar para concatenar cadenas de texto y valores de forma más concisa.

```python
nombre = "NicLau"
edad = 15

print(f"Hola, mi nombre es {nombre} y tengo {edad} años.")
```
Sol: Hola, mi nombre es *NicLau* y tengo *15* años.  

## Tipos de datos en Python.
En Python, un tipo de dato se refiere a la *clasificación de los valores que pueden ser almacenados en una variable*. Cada tipo de dato tiene características y propiedades específicas que lo hacen adecuado para ciertos usos y operaciones.  

Los tipos de datos en Python se pueden dividir en dos categorías principales:

* **Tipos básicos**: son los tipos de datos más simples y fundamentales.  
* **Tipos compuestos**: son tipos de datos que se basan en otros tipos de datos básicos.

### **Tipos básicos**.  
* **Textos (String)**: representan cadenas de caracteres.

* **Númericos**: representan números. Los tipos numéricos en Python son:  
  * **Enteros (int)**: representan números enteros, positivos o negativos.
  * **Punto flotante (float)**: representan números con decimales.
  * **Complejos (complex)**: representan números complejos, que son la suma de un número real y un número imaginario.

* **Booleanos**: representan valores lógicos, verdaderos (True) o falsos (False).

### **Tipos compuestos**.
* **Secuencias**: representan colecciones de datos ordenados. Los tipos de secuencias en Python son:
  * **Listas (list)**: representan colecciones mutables de datos.
  * **Tuplas (tuple)**: representan colecciones inmutables de datos.
  * **Rangos (range)**: representan secuencias de números.
* **Mapas (map)**: representan asociaciones entre claves y valores.
  * **Diccionarios (dictionaries)**: se utilizan para almacenar valores de datos en pares claves:valor.  
* **Conjuntos**: representan colecciones de datos sin elementos duplicados.

### Función type().
Para poder descubrir el tipo de dato de una variable, Python nos ofrece la función ***type()***. La sintaxis de la función es la siguiente:

```python
type(objeto)
```

```python
#Definimos variables y le asignamos valores.
numero_entero = 7
numero_decimal = 7.7
temperatura = 24.5
numero_complejo = 1 + 2j
texto = "hola"

#Salida y tipo de dato:
print(type(numero_entero))
print(type(numero_decimal))
print(type(temperatura))
print(type(numero_complejo))
print(type(texto))
```
Sol:  
class 'int'  
class 'float'  
class 'float'  
class 'complex'  
class 'str'  

### **Operaciones con tipos de datos**.

Los tipos de datos en Python pueden ser operados entre sí mediante diferentes tipos de operaciones. Las operaciones más comunes son:  

* **Operaciones aritméticas**: se utilizan para realizar operaciones aritméticas básicas, como suma, resta, multiplicación, división y potenciación.  

* **Operaciones lógicas**: se utilizan para realizar operaciones lógicas básicas, como AND, OR y NOT.  

* **Operaciones de comparación**: se utilizan para comparar valores de diferentes tipos de datos.

## Operadores Aritméticos.

| Operador | Descripción |
| :------: | :------: |
| + | Suma |
| - | Resta |
| * | Multiplicación |
| / | División |
| ** | Potenciación |
| // | División entera |
| % | Módulo |

En Python, las operaciones aritméticas **se realizan de izquierda a derecha**, pero hay algunos operadores que tienen una prioridad mayor que otros. La siguiente tabla muestra la prioridad de los operadores aritméticos en Python:  

| Operador | Prioridad |
| :------: | :-------: |
| ** | 1 |
| * | 2 |
| / | 2 |
| // | 2 |
| % | 2 |
| + | 3 |
| - | 3 |

Si los operadores siguen unas ***reglas de precedencia*** que determinan su orden de aplicación, que hacer cuando deseamos un orden de aplicación distinto? ***usar paréntesis***, como hacemos en la notación matemática convencional.

```python
# Definimos dos variables.
x = 2
y = 1

# Operación suma asignada a una variable.
z = x + y  
r = x - y  
m = x * y  
d = x / y
p = x ** y 

# Salida
print(z)  
print(r)  
print(m)  
print(d)
print(p)   
```
Sol:  
3  
1  
2  
2  
2  

## Conversión de datos.
En programación, la conversión de tipos de datos es el proceso de cambiar un valor de un tipo de datos a otro. Esto puede ser necesario para realizar operaciones o funciones que requieren un tipo de datos específico.  

En Python, la conversión de tipos de datos se puede realizar de forma explícita o implícita.

### Conversión explícita.

La conversión explícita de tipos de datos se realiza utilizando funciones o métodos especiales. Las funciones y métodos más comunes para la conversión de tipos de datos en Python son:  

* **int()**: convierte un valor a un entero.
* **float()**: convierte un valor a un número de punto flotante.
* **str()**: convierte un valor a una cadena de texto.
* **bool()**: convierte un valor a un valor booleano.

### Convertir dato tipo str a int.
```python
# Valores introducidos por el usuario, convertimos de un tipo de dato string a integer, y asignamos cada valor a una variable:
x = int(input("Introduce un valor para 'x': "))
y = int(input("Introduce un valor para 'y': "))

# Imprimimos la operación aritmética:
print(x + y)
```
Sol:  
Introduce un valor para 'x': 1 (introducido por el usuario)  
Introduce un valor para 'y': 2 (introducido por el usuario)  
3  

```python
# Valores introducidos por el usuario, y cada uno asignados a una variable:
x = input("Introduce un valor para 'x': ")
y = input("Introduce un valor para 'y': ")

# Operación suma asignada a una variable, convertimos a dato tipo enteros cada valor introducido por el usuario:
z = int(x) + int(y)

# Salida:
print(z)
```
Sol:  
Introduce un valor para 'x': 1 (introducido por el usuario)  
Introduce un valor para 'y': 2 (introducido por el usuario)  
3    

### Convertir dato tipo str a float.
```python
# Valores introducidos por el usuario, convertimos de un tipo de dato string a float, y asignamos cada valor a una variable:
x = float(input("Introduce un valor para 'x': "))
y = float(input("Introduce un valor para 'y': "))

# Imprimimos la operación aritmética:
print(x + y)
```
Sol:  
Introduce un valor para 'x': 1.2 (introducido por el usuario)  
Introduce un valor para 'y': 3.4 (introducido por el usuario)  
4.6  


En Python, la función **round()** se utiliza para *redondear un número a un número entero o a un número decimal* con una precisión determinada. La sintaxis de la función es la siguiente:

```python
round(número, ndigitos)
```

*número* es el número que se desea redondear, *ndigitos* es el número de decimales a los que se desea redondear el número. Por defecto, ndigitos es 0, lo que significa que el número se redondea al número entero más cercano.  

En Python, también existe la función **math.floor()**, que redondea un número **hacia abajo**, y la función **math.ceil()**, que redondea un número **hacia arriba**. La sintaxis de estas funciones es la siguiente:  

```python
math.floor(número)
```

```python
math.ceil(número)
```

```python
x = float(input("Introduce un valor para 'x': "))
y = float(input("Introduce un valor para 'y': "))

# Función de redondeo.
print(round(x + y))
```
Sol:  
Introduce un valor para 'x': 2  
Introduce un valor para 'y': 4.6  
7  

```python
x = float(input("Introduce un valor para 'x': "))
y = float(input("Introduce un valor para 'y': "))

z = round(x + y)

print(f"{z:,}")
```
Sol: 1,000  

```python
x = float(input("Introduce un valor para 'x': "))
y = float(input("Introduce un valor para 'y': "))

z = x / y

print(z)
```
Sol: 0.6666666666666666  

```python
x = float(input("Introduce un valor para 'x': "))
y = float(input("Introduce un valor para 'y': "))

z = round(x / y, 2)      # Redondear a 2 decimales.

print(z)
```
Sol: 0.67  

Otra manera de hacerlo es la siguiente:
```python
x = float(input("Introduce un valor para 'x': "))
y = float(input("Introduce un valor para 'y': "))

z = x / y

print(f"{z:.2f}")   # z:.2f indica que del resultado para z, mostrará 2 decimales.
```
Sol: 0.67  

## Definir una función en Python.
En Python, una *función es un bloque de código que se puede reutilizar simplemente llamando a la función*. Esto permite la reutilización de código simple y elegante sin volver a escribir explícitamente secciones de código.  

Para definir una función en Python, se utiliza la palabra clave **def**. A continuación viene el **nombre o identificador de la función** que es el que se utiliza para invocarla. Después del nombre hay que incluir los **paréntesis** y una lista opcional de parámetros.  

Los **parámetros** de una función *son valores que se pueden pasar a la función cuando se llama*. Los parámetros pueden ser de cualquier tipo, incluidos números, cadenas, listas, etc.

El valor de **retorno (return)** de una función es el *valor que se devuelve cuando la función se completa*. El valor de retorno puede ser de cualquier tipo, incluidos números, cadenas, listas, etc.

```python
# Definimos una función que genera un saludo.
# Definimos una función, con x como parámetro:
def hello(x):
    print("Hola", x)

# Definimos una variable que tendra como valor la información obtenida desde el usuario. 
name = input("Cual es tu nombre?: ")
# La función hello toma como parámetro la variable name, la cual, sera el valor del parámetro x. 
hello(name)
```
Sol: Cual es tu nombre?: *NicLau*  
Hola *NicLau*

```python
# Definimos una función que genera un saludo.
# Definimos una función, con x como parámetro:
def hello(x = "mundo"):
    print("Hola", x)

#Llamamos la función hello.
hello()

# Definimos una variable que tendra como valor la información obtenida desde el usuario. 
name = input("Cual es tu nombre?: ")
# La función hello toma como parámetro la variable name, la cual, sera el valor del parámetro x. 
hello(name)
```
Sol:  
Hola mundo  
Cual es tu nombre?: *NicLua*  
Hola *NicLau*  

```python
# Definimos una función que realiza la operación de sumar dos números.
def sumar(a, b):
  """
  Suma dos números.

  Argumentos:
    a: El primer número.
    b: El segundo número.

  Retorna:
    La suma de los dos números.
  """
  return a + b

# Definir una variable que contenga el resultado de la funcion suma:
resultado = sumar(1,2)
print(resultado)
```
Sol: 3  

```python
# Programa que calcula el cuadrado de cualquier número.
# Función principal:
def main():
   x = int(input("Cual es el valor de x: "))
   print("El cuadrado de x es", cuadrado(x))

# Función que permite calcular el cuadrado de cualquier número:
def cuadrado(n):
   return n ** 2

# Invocamos o llamamos la función:
main()
```
Sol:  
Cual es el valor de x: *3*  
9  

