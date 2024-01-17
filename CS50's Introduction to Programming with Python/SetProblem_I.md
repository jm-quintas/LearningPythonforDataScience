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
