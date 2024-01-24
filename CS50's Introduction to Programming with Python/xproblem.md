## Proyecto 1.
Crear un progrma que pregunte al usuario información sobre su nombre, ciudad donde nació, nombre de su mascota y su banda de música favorita. Luego combinar toda la información en un mensaje de salida.

```python
# Saludo de bienvenida:
print("Bienvenido a nuestro programa!")

# Preguntar el nombre:
nombre = input("Introduce tu nombre: ")

# Preguntar la ciudad donde nacio:
ciudad = input("Introduce la ciudad donde naciste: ")

# Preguntar el nombre de su mascota:
mascota = input("Introduce el nombre de tu mascota: ")

# Banda de música:
banda = input("Banda de música: ")

# Combinar información y mostrar salida:
print(f"Hola {nombre}, naciste en {ciudad}, tu mascota se llama {mascota} y tu banda de música favorita es {banda}.")
```
Sol:  
Bienvenido a nuestro programa!    
Introduce tu nombre: ***NicLau***  
Introduce la ciudad donde naciste: ***Maracaibo***  
Introduce el nombre de tu mascota: ***Jacob***  
Banda de música: ***Maná***          
Hola ***NicLau***, naciste en ***Maracaibo***, tu mascota se llama ***Jacob*** y tu banda de música favorita es ***Maná***. 

## Proyecto 2.
Crear dos variables que contengan información por parte del usuario:
   * Primera variable llamada ***pais***.
   * Segunda variable llamada ***continente***.
Mostrar un mensaje por pantalla que combine las dos variables, y crear comentarios que resalten el tipo de variable.

```python
# Variables.
pais = input("Introduce tu país: ")
continente = input("En que continente se encuentra tu país: ")

# Combinamos las variables en un solo mensaje:
print(f"Hola eres de {pais}, que se encuentra en el continente de {continente}.")

# Demostrar el tipo de variable (string):
print(type(pais))
print(type(continente))
```
Sol:  
Introduce tu pais: ***Venezuela***  
En que continente se encuentra tu pais: ***Latinoamerica***  
Hola eres de ***Venezuela***, que se encuentra en el continente de ***Latinoamerica***.  
<class 'str'>  
<class 'str'>  
