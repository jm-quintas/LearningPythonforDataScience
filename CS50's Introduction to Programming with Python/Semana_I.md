# Funciones y Variables.

## Archivos en Python.
Todos los programas que se escriben en lenguaje Python se deben guardar en un archivo con extención .py con la finalidad de indicarle a la computadora que efectivamente estamos trabajando en un programa de Python.

```python{
nombre_archivo.py
```

Para ejecutar el programa debemos utilizar la siguiente sintaxis en la terminal o consola de comando:

```{python}
python nombre_archivo.py
```

## Funciones incorporadas en Python.
Python incluye una gran cantidad de funciones incorporadas que se pueden utilizar sin necesidad de definirlas. Su sintaxis es la siguiente:  

```{python}
nombre_funcion_python(argumento)
```

Los *argumentos* son una entrada a una función que de alguna manera influye en su comportamiento. En la mayoria de las ocaciones los argumentos deben ir encerrados entre comillas.

```{python}
nombre_funcion_python("argumento")
```

### **Función print()**.
Imprime un mensaje en la terminal o consola de comandos.

```{python}
print("Hola, mundo")
```
Sol: Hola, mundo  

### **Función input()**.
Se utiliza para solicitar al usuario que *introduzca datos por teclado*. La función **input() devuelve una cadena de texto**, por lo que es necesario convertirla al tipo de datos deseado. Su sintaxis es la siguiente:

```{python}
input(prompt)
```

El **prompt** es una cadena de texto que se muestra al usuario para solicitar la entrada.

```{python}
input("Cual es tu nombre: ")
```
Sol: Cual es tu nombre: 

Más adelante estudiaremos otras funciones incorporadas en el lenguaje de Python.  

## Variables.
En Python, las *variables son nombres que se utilizan para almacenar valores en la memoria del ordenador*. Permiten guardar información para utilizarla posteriormente en el código.  

Características principales de las variables en Python:

* **No es necesario declararlas**: A diferencia de otros lenguajes, *en Python no se necesita declarar el tipo de dato de una variable* antes de usarla. El tipo se asigna automáticamente cuando se le asigna un valor por primera vez.
  
* **Tipado dinámico**: Python *es un lenguaje de tipado dinámico*, lo que significa que el tipo de dato de una variable puede cambiar a lo largo del programa.
  
* **Nombres significativos**: Es recomendable *utilizar nombres descriptivos para las variables*, que indiquen claramente qué tipo de información almacenan.
  
* **Sensibilidad a mayúsculas y minúsculas**: Python distingue entre mayúsculas y minúsculas en los nombres de las variables. Por ejemplo, nombre y NOMBRE son variables diferentes.

