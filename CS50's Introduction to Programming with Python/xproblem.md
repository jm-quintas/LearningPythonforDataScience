## Proyecto 1. Mensaje.
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

## Proyecto 2. Mensaje.
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

## Proyecto 4. Evaluar expresiones.
¿Qué resultados se obtendrán al evaluar las siguientes expresiones Python?  
a) int(exp(2 * log(3)))  
b) round(4*sin(3 * pi / 2))  
c) abs(log10(.01) * sqrt(25))  
d) round(3.21123 * log10(1000), 3)  

```python
from math import exp, sin, log, log10, sqrt

# Parte a:
expresion1 = int(exp(2 * log(3)))
print(expresion1)

# Parte b:
pi = 3.1415
expresion2 = round(4 * sin((3 * pi) / 2))
print(expresion2)

# Parte 3:
expresion3 = abs(log10(.01) * sqrt(25))
print(expresion3)

# Parte 4:
expresion4 = round(3.21123 * log10(1000), 3)
print(expresion4)
```
Sol:  
9  
-4  
10.0  
9.634  

## Proyecto 5. Área y perímetro de un cuadrado.
Diseña un programa que, a partir del valor del lado de un cuadrado (3 metros), muestre el valor de su perímetro (en metros) y el de su área (en metros cuadrados). (El perímetro debe darte 12 metros y el área 9 metros cuadrados).

```python
# Entrada de datos:
lado = float(input("Introduce un valor para el lado: "))

# Ecuaciones:
perimetro_cuadrado = lado + lado + lado + lado

area_cuadrado = lado * lado

print(f"El perímetro del cuadrado es: {perimetro_cuadrado} metros")
print("El área del cuadrado es: {} metros cuadrados".format(area_cuadrado))
```
Sol:  
Introduce un valor para el lado: ***3***   
El perímetro del cuadrado es: ***12.0*** metros  
El área del cuadrado es: ***9.0*** metros cuadrado  

## Proyecto 6. Área de un triángulo.
Diseña un programa que, a partir del valor de la base y de la altura de un triángulo (3 y 5 metros, respectivamente), muestre el valor de su área (en metros cuadrados). Recuerda que el área A de un triángulo se puede calcular a partir de la base b y la
altura h como A = (1/2)bh.  

```
# Introducimos valores para las variables base y altura:
base = float(input("Introduce el valor para la base: "))
altura = float(input("Introduce el valor para la altura: "))

# Ecuación:
area = (1/2) * base * altura

# Salida:
print(f"El área del tiángulo es: {area} metros cuadrados")
```
Sol:  
Introduce el valor para la base: ***3***  
Introduce el valor para la altura: ***5***  
El área del tiángulo es: ***7.5*** metros cuadrados  

