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

## Proyecto 7. Área y perímetro de un rectángulo.
Diseña un programa que, a partir del valor de los dos lados de un rectángulo (4 y 6 metros, respectivamente), muestre el valor de su perímetro (en metros) y el de su área (en metros cuadrados). El perímetro debe darte 20 metros y el área 24 metros cuadrados.  

```python
# Introducimos valores para las variables base y altura:
longitud = float(input("Introduce el valor para la longitud: "))
ancho = float(input("Introduce el valor para el ancho: "))

# Ecuación:
area = longitud * ancho
perimetro = 2 * longitud + 2 * ancho

# Salida:
print(f"El área del rectángulo es: {area} metros cuadrados")
print(f"El perímetro del rectángulo es: {perimetro} metros")
```
Sol:  
Introduce el valor para la longitud: ***4***   
Introduce el valor para el ancho: ***6***  
El área del rectángulo es: ***24.0*** metros cuadrados  
El perímetro del rectángulo es: ***20.0*** metros  

## Proyecto 8. Área de un triángulo.
El área ***A*** de un triángulo se puede calcular a partir del valor de dos de sus lados, ***a*** y ***b***, y del ángulo ***θ*** que estos forman entre sí con la fórmula ***A = (1/2)absenθ***. Diseña un programa que pida al usuario el valor de los dos lados (en metros), el ángulo que estos forman (en grados), y muestre el valor del área. Ten en cuenta que la función ***sin*** de Python trabaja en radianes, así que el ángulo que leas en grados deberas pasarlo a radianes sabiendo que ***π*** radianes son ***180 grados***. Prueba que has hecho bien el programa introduciendo los siguientes datos: ***a = 1***, ***b = 2***, ***θ = 30***; el resultado es ***0.5***).  

```python
# Importar desde la libreria.
from math import sin 

# Introducimos valores para las variables base y altura:
lado_a = float(input("Introduce un valor para el lado a: "))
lado_b = float(input("Introduce un valor para el lado b: "))

# Introducimos valores para el ángulo:
angulo = float(input("Introduce un valor para el ángulo: "))

# Conversión de ángulo:
nuevo_angulo = (angulo * 3.1415) / 180

# Ecuación:
area = (1/2) * lado_a * lado_b * sin(nuevo_angulo)

# Salidas:
print(nuevo_angulo)
print(f"El área del triángulo es: {area} metros cuadrado")
```
Sol:  
Introduce un valor para el lado a: ***1***  
Introduce un valor para el lado b: ***2***  
Introduce un valor para el ángulo: ***30***  
El ángulo es: ***0.5235833333333334***  
El área del triángulo es: ***0.49998662654663256*** metros cuadrado   

## Proyecto 9. Capital - Interés - Año.
Haz un programa que pida al usuario una cantidad de euros, una tasa de interés y un número de años. Muestra por pantalla en cuanto se habra convertido el capital inicial transcurridos esos años si cada año se aplica la tasa de interés introducida. Recuerda que un capital de ***C*** euros a un interés del ***x*** por cien durante ***n*** años se convierten en ***C(1 + x/100)^n*** euros. Prueba tu programa sabiendo que una cantidad de 10,000 euros al 4.5% de interés anual se convierte en 24117.14 euros al cabo de 20 años.  

```python
# Entrada de valores:
cantidad_euro = float(input("Introduce una cantidad de euros: "))
tasa_interes = float(input("Introduce una cantidad de intéres: "))
anos = int(input("Introduce una cantidad de años: "))

# Cálculo:
capital = cantidad_euro * (1 + tasa_interes / 100) ** anos

# Salida:
print(f"Cantidad de dinero: {capital} euros")
```
Sol:  
Introduce una cantidad de euros: ***10000***  
Introduce una cantidad de intéres: ***4.5***  
Introduce una cantidad de años: ***20***  
Cantidad de dinero: ***24117.140248374057*** euros  

## Proyecto 10. Área y perímetro de una círcunferencia.
Diseña un programa que solicite el radio de una circunferencia y muestre su área y perímetro con sólo 2 decimales.

```python
# Entrada de valores:
radio = float(input("Introduce un valor para el radio: "))

# Definimos una constante:
pi = 3.1415

# Cálculo:
area_circunferencia = pi * (radio ** 2)
area_redondeada = round(area_circunferencia, 2)

perimetro_circunferencia = 2 * pi * radio
perimetro_redondeado = round(perimetro_circunferencia, 2)

# Salida:
print(f"El área de la circunferencia es: {area_redondeada} metros cuadrados")
print(f"El perímetro de la circunferencia es: {perimetro_redondeado} metros")
```
Sol:  
Introduce un valor para el radio: ***3***  
El área de la circunferencia es: ***28.27*** metros cuadrados  
El perímetro de la circunferencia es: ***18.85*** metros  

## Proyecto 11. Función lineal y su gráfica.
Gráficar la siguiente función lineal: y = 2x + 1, equivale a la función y = mx + b.

```python
# Librerias para graficar:
import numpy as np
import matplotlib.pyplot as plt

# Función lineal:
x = np.arange(-3,4)
y = 2*x + 1

# Gráfica:
plt.plot(x,y)
plt.xlabel("Eje x")
plt.ylabel("Eje y")
plt.title("Gráfica de función lineal")
plt.show()
```
Sol:  
![](https://github.com/jm-quintas/LearningPythonforDataScience/blob/main/CS50's%20Introduction%20to%20Programming%20with%20Python/Gr%C3%A1fica%20lineal.png)

## Proyecto 12. Función cuadrática y su gráfica.
Gráficar la siguiente función cuadrática: y = x^2.

```python
#Librerias:
import numpy as np
import matplotlib.pyplot as plt

# Función cuadrática:
x = np.arange(-5, 6)
y = x**2

# Gráfica:
plt.plot(x, y, 'g-o')
plt.xlabel('Eje x')
plt.ylabel('Eje y')
plt.title('Gráfica de una función cuadrática')
plt.show()
```
Sol:  
![](https://github.com/jm-quintas/LearningPythonforDataScience/blob/main/CS50's%20Introduction%20to%20Programming%20with%20Python/Gr%C3%A1fica%20cuadr%C3%A1tica.png)

## Proyecto 12. Cálculo de velocidad y su gráfica.
Una motocicleta inicia un recorrido con una velocidad de 8 m/s y una aceleración constante de 0.15 m/s^2, si su desplazamiento dura 29 segundos. Determine su velocidad final.

```python
# Librerias:
import numpy as np
import matplotlib.pyplot as plt

# Información:
t = np.arange(0, 30)
vi = 8
acel = 0.15

# Ecuación:
vf = vi + acel*t

# Resultado
print(f"La velocidad final de la motocicleta es: {vf} m/s")

# Gráfica:
plt.plot(t, vf, 'r-o')
plt.xlabel('tiempo(s)')
plt.ylabel('Velocidad(m/s)')
plt.title('Gráfica velocidad vs tiempo')
plt.show()
```
Sol:  
![](https://github.com/jm-quintas/LearningPythonforDataScience/blob/main/CS50's%20Introduction%20to%20Programming%20with%20Python/Gr%C3%A1fica%20velocidad.png)
