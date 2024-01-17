```python
"""

Implemente un programa que solicite al usuario la respuesta a la Gran Pregunta de la Vida,
el Universo y Todo, generando 'Yes' si el usuario ingresa 42 o (sin distinguir entre mayúsculas
y minúsculas) 'forty-twoo' 'forty two'. De lo contrario, salida 'No'.

"""

respuesta = input("What is the Answer to the Great Question of Life, the Universe, and Everything?:" )

respuesta_transf = respuesta.lower()

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

respuesta_transf = respuesta.lower()

if respuesta_transf == "42" or respuesta_transf == "forty-two" or respuesta_transf == "forty two":
    print("Yes")

else:
    print("No")
```
Sol:  
What is the Answer to the Great Question of Life, the Universe, and Everything?: *forty-two*  
Yes  
