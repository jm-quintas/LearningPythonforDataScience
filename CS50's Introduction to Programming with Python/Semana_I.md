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
