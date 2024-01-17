## Problema 1: pensamiento profundo.
```python
"""

Implemente un programa que solicite al usuario la respuesta a la Gran Pregunta de la Vida,
el Universo y Todo, generando 'Yes' si el usuario ingresa 42 o (sin distinguir entre mayúsculas
y minúsculas) 'forty-twoo' 'forty two'. De lo contrario, salida 'No'.

"""

respuesta = input("What is the Answer to the Great Question of Life, the Universe, and Everything?:" )

respuesta_transf = respuesta.lower().strip()

if respuesta_transf == "42":
    print("Yes")
elif respuesta_transf == "forty-two":
    print("Yes")
elif respuesta_transf == "forty two":
    print("Yes")
else:
    print("No")
```
Sol:  
What is the Answer to the Great Question of Life, the Universe, and Everything?: *42*  
Yes  

```python
respuesta = input("What is the Answer to the Great Question of Life, the Universe, and Everything?:" )

respuesta_transf = respuesta.lower().strip()

if respuesta_transf == "42" or respuesta_transf == "forty-two" or respuesta_transf == "forty two":
    print("Yes")

else:
    print("No")
```
Sol:  
What is the Answer to the Great Question of Life, the Universe, and Everything?: *forty-two*  
Yes  

## Problema 2: inicio Caja Federal de Ahorros.
```python
"""

Implemente un programa que solicite un saludo al usuario. Si el saludo comienza con "hola", envíe $0. Si el saludo 
comienza con una “h” (pero no “hola”), envíe $20. De lo contrario, genere $100.
Ignore cualquier espacio en blanco inicial en el saludo  del usuario y trate el saludo del usuario sin distinguir entre mayúsculas y minúsculas.

"""

saludo = input("Saludo: ")

saludo_transf = saludo.lower().strip()

if saludo_transf == "hola":
    print("0$")

else:
    if saludo_transf.startswith("h"):
        print("20$")
    else:
        print("100$")
```
Sol:  
Saludo: *hola*  
0$  

```python
saludo = input("Saludo: ")

saludo_transf = saludo.lower().strip()

if saludo_transf == "hola":
    print("0$")

elif saludo_transf:
    if saludo_transf.startswith("h"):
        print("20$")
    else:
        print("100$")
```
Sol:  
Saludo: *NicLau*  
100$  

## Problema 3: Extensiones de archivo.
```python
"""

Implemente un programa que solicite al usuario el nombre de un archivo y luego genere 
el tipo de medio de ese archivo si el nombre del archivo termina, sin distinguir entre
mayúsculas y minúsculas, en cualquiera de estos sufijos:

* .gif
* .jpg
* .jpeg
* .png
* .pdf
* .txt
* .zip

"""

nombre_archivo = input("Nombre del archivo: ")

nombre_archivo_transf = nombre_archivo.lower().strip()

# Condicional:
if nombre_archivo_transf.endswith("gif"):
    print("image/gif")
elif nombre_archivo_transf.endswith("jpg"):
    print("image/jpeg")
elif nombre_archivo_transf.endswith("jpeg"):
    print("image/jpeg")
elif nombre_archivo_transf.endswith("png"):
    print("image/png")
elif nombre_archivo_transf.endswith("pdf"):
    print("application/pdf")
else:
    print("application/octet-stream")
```
Sol:  
Nombre del archivo: cat.gif  
image/gif  


## Prolema 4: Intérprete de matemáticas.
```python
"""

Implemente un programa que solicite al usuario una expresión aritmética 
y luego calcule y genere el resultado como un valor de punto flotante formateado
con un decimal. Supongamos que la entrada del usuario tendrá el formato x y z, 
con un espacio entre xy y un espacio entre yz, donde:

x es un número entero
y es +, -, *, o/
z es un número entero

"""
# Entrada de datos:
expresion = input("Expression: ")

# Asignación del valores transformados:
x, y, z = expresion.split(" ")

# Cambiamos el tipo de datos y la asignamos a una nueva variable:
nueva_x = float(x)
nueva_z = float(z)

# Condicionales y calculamos el resultado:
if y == "+":
    print(nueva_x + nueva_z)
elif y == "-":
    print(nueva_x - nueva_z)
elif y == "*":
    print(nueva_x * nueva_z)
else:
    print(nueva_x / nueva_z)
```
Sol:  
Expression: 1 + 1  
2.0  

Expression: 2 - 3  
-1.0  

Expression: 2 * 2  
4.0  

Expression: 50 / 5  
10.0  
