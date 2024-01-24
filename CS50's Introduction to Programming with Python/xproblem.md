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

## Proyecto 3. Evaluar polinomio.
Evalúa el polinomio x^4 + x^3 + 2x^2 - x en x = 1.1. Utiliza variables para evitar teclear varias veces el valor de x. El resultado es 4.1151.

```python
# Definimos una variable:
x = 1.1

# Polinomio:
p = x**4 + x**3 + 2 * (x**2) - x

# Salida y redondeo:
print(round(p, 4))
```
Sol:  
4.1151  

Evalúa el polinomio x^4 + x^3 + (1/2)x^2 - x en x = 10. Asegúrate de que el resultado sea un número flotante. El resultado es 11040.0.  

```python
# Definimos una variable:
x = 10

# Polinomio:
p = x**4 + x**3 + (1/2) * (x**2) - x

# Salida y redondeo:
print(float(p))
```
Sol:  
11040.0  

