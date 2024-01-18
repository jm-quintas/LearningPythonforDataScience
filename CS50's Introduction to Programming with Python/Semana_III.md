# Bucles en Python.

En Python, los ***bucles*** se utilizan para *repetir una porción de código tantas veces como sea necesario*. Hay dos tipos de bucles en Python:  

* **Bucle while**: repite el código mientras la condición sea verdadera.  
* **Bucle for**: repite el código para cada elemento de una colección.  

## Bucle While.
Es una estructura de control de flujo que ***se utiliza para repetir un bloque de código mientras se cumple una condición determinada***. La condición es una expresión booleana que se evalúa en cada iteración. En otras palabras, ***se ejecutará el bloque de código mientras la condición sea verdadera, es decir True***. Seguirá ejecutándose hasta que el valor booleano de la condición deje de ser verdadero. La sintaxis básica de un bucle while es la siguiente:  

```python
while condición:
    # Código que se repite
```

```python
# Iniciamos la variable, y asignamos un valor.
i = 3

# Uso del bucle while.
while i != 0:
    print("meow")
    # Actualización de la variable de iteración.
    i = i - 1
```
Sol:  
meow  
meow  
meow  
