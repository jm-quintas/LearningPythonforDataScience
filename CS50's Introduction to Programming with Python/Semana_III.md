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

```python
i = 0
while i != 3:
    print("meow")
    i = i + 1
```
Sol:  
meow  
meow  
meow  

```python
i = 1
while i <= 3:
    print("meow")
    i = i + 1
```
Sol:  
meow  
meow  
meow  

```python
i = 0
while i < 3:
    print("meow")
    # i += 1
    i = i + 1
```
Sol:  
meow  
meow  
meow  

## Bucle for.
Se usa cuando se conoce de antemano el ***número de veces que se debe repetir el código***. El código se repite para cada elemento de una colección. La sintaxis básica de un bucle ***for*** es la siguiente:

```python
for elemento in colección:
    # Código que se repite
```
### Listas.
En Python, una lista es un ***tipo de dato secuencial*** que se utiliza para ***almacenar una colección de datos del mismo o de diferentes tipos***. Las listas son mutables, lo que significa que sus elementos se pueden modificar después de haber sido creadas. Su sintaxis es la siguiente:

```python
lista = [elemento 1, elemento 2, elemento 3, elemento n]
```

```python
"""
Por cada elemento que la variable de iteración pase por la lista
imprimirá un meow.
"""
for i in [0, 1, 2]:
    print("meow")
```

### Rangos.
La función ***range()*** en Python se utiliza para ***crear una secuencia de números***. La secuencia de números puede ser de cualquier longitud, y puede comenzar en cualquier número.

La sintaxis básica de la función range() es la siguiente:  
```python
range(inicio, fin, [paso])
```
Los argumentos de la función range() son los siguientes:

* **Inicio**: el primer número de la secuencia. El valor predeterminado es 0.
* **Fin**: el último número de la secuencia. El número fin no se incluye en la secuencia.
* **Paso**: el incremento entre los números de la secuencia. El valor predeterminado es 1.

```python
for i in range(3):
    print("meow")
```
Sol:  
meow   
meow    
meow  

```python
while True:
    n = int(input("Cual es el valor de n?"))
    if n > 0:
        break

for i in range(n):
    print("meow")
```
Sol: 
meow   
meow    
meow  

Trabajando con funciones creadas y bucles:  

```python
def main():
    meow(3)

def meow(n):
    for i in range(n):
        print("meow")

main()
```
Sol:  
meow   
meow    
meow 

Trabajando con funciones, condicionales y bucles:  

```python
def main():
    number = get_number()
    meow(number)

# Función que se encarga de obtener información de parte del usuario:
def get_number():
    while True:
        n = int(input("Cual es el valor de n? "))
        if n > 0:
            break
    return n

# Función que se encarga de imprimir el número de veces el mensaje:
def meow(n):
    for i in range(n):
        print("meow")

# Llamada de la función principal, salida:
main()
```
Sol:  
Cual es el valor de n? *3*  
meow   
meow    
meow  

Trabajando con listas:  
```python
estudiantes = ["Harry", "Hermione", "Ron"]
print(estudiantes)
```
Sol: ['Harry', 'Hermione', 'Ron']  
