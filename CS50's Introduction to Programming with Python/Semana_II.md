# Condicionales en Python.

## Condicionales.
En Python, las sentencias condicionales *se usan para controlar el flujo del programa*. Permiten ejecutar código solo si se cumple una condición determinada.  

Hay tres tipos básicos de sentencias condicionales en Python:  

* ***Sentencia if***: se usa para ejecutar código si una condición es verdadera. La sentencia ***if*** tiene la siguiente sintaxis:

```python
 if condición:
    bloque de código
```
Si la condición es verdadera, se ejecutará el bloque de código. Si la condición es falsa, no se ejecutará el bloque de código.
  
* ***Sentencia if-else***: se usa para ejecutar código si una condición es verdadera o código diferente si la condición es falsa. La sentencia ***if-else*** tiene la siguiente sintaxis:

 ```python
if condición:
    bloque de código verdadero
else:
    bloque de código falso
```
Si la condición es verdadera, se ejecutará el bloque de código verdadero. Si la condición es falsa, se ejecutará el bloque de código falso.
  
* ***Sentencia if-elif-else***: se usa para ejecutar código si una condición es verdadera, código diferente si otra condición es verdadera, o código diferente si ninguna de las condiciones es verdadera. La sentencia ***if-elif-else*** tiene la siguiente sintaxis:

```python
if condición 1:
    bloque de código 1
elif condición 2:
    bloque de código 2
else:
    bloque de código 3
```
Si la condición 1 es verdadera, se ejecutará el bloque de código 1. Si la condición 1 es falsa y la condición 2 es verdadera, se ejecutará el bloque de código 2. Si las condiciones 1 y 2 son falsas, se ejecutará el bloque de código 3.

## Operadores condicionales.
En Python, los operadores condicionales se usan para evaluar condiciones. Las condiciones son expresiones que pueden evaluarse como verdaderas o falsas. Los operadores condicionales básicos en Python son los siguientes:

| Operador | Descripción |
| :------: | :------: |
| == | Igualdad |
| != | Desigualdad |
| < | Menor que |
| > | Mayor que |
| <= | Menor o igual que |
| >= | Mayor o igual que |

## Operadores lógicos.
Los operadores lógicos se usan para combinar condiciones. Los operadores lógicos básicos en Python son los siguientes:

| Operador | Descripción |
| :------: | :------: |
| and | Y |
| or | O |
| not | No |

### Aplicando los conceptos de condicionales.
```python
# Comprobar si un valor es mayor, menor o igual a otro.
# Valores por parte del usuario almacenados en sus respectivas variables.
x = int(input("Introduce un valor para x: "))
y = int(input("Introduce un valor para y: "))

# Aplicando la condicional if:
if x < y:
    print("x es menor que y")

if x > y:
    print("x es mayor que y")

if x == y:
    print("x es igual a y")
```
Sol:  
Introduce un valor para x: *1*  
Introduce un valor para y: *2*  
x es menor que y  

```python
# Comprobar si un valor es mayor, menor o igual a otro.
# Valores por parte del usuario almacenados en sus respectivas variables.
x = int(input("Introduce un valor para x: "))
y = int(input("Introduce un valor para y: "))

# Aplicando la condicional if, elif:
if x < y:
    print("x es menor que y")

elif x > y:
    print("x es mayor que y")

elif x == y:
    print("x es igual a y")
```
Introduce un valor para x: *1*  
Introduce un valor para y: *2*  
x es menor que y  

```python
# Comprobar si un valor es mayor, menor o igual a otro.
x = int(input("Introduce un valor para x: "))
y = int(input("Introduce un valor para y: "))

# Aplicando las condiciones if, elif, else:
if x < y:
    print("x es menor que y")

elif x > y:
    print("x es mayor que y")

else:
    print("x es igual a y")
```
Sol:  
Introduce un valor para x: *2*  
Introduce un valor para y: *2*  
x es igual a y  

```python
# Comprobar si los valores numéricos ingresados son iguales o distintos.
x = int(input("Introduce un valor para x: "))
y = int(input("Introduce un valor para y: "))

if x < y or x > y:
    print("x no es igual a y")

else:
    print("x es igual a y")
```
Sol:  
Introduce un valor para x: *3*  
Introduce un valor para y: *5*  
x no es igual a y  

```python
# Comprobar si los valores numéricos ingresados son iguales o distintos.
x = int(input("Introduce un valor para x: "))
y = int(input("Introduce un valor para y: "))

if x != y:
    print("x no es igual a y")

else:
    print("x es igual a y")
```
Sol:  
Introduce un valor para x: *5*  
Introduce un valor para y: *5*  
x es igual a y  

```python
# Comprobar si los valores numéricos ingresados son iguales o distintos.
x = int(input("Introduce un valor para x: "))
y = int(input("Introduce un valor para y: "))

if x == y:
    print("x es igual a y")
else:
    print("x es distinto a y")
```
Sol:  
Introduce un valor para x: *7*  
Introduce un valor para y: *7*  
x es igual a y  

```python
# Conversión de notas académicas.
nota = int(input("Introduce una nota: "))

if nota >= 90 and nota <= 100:
    print("nota: A")

elif nota >=80 and nota < 90:
    print("nota: B")

elif nota >= 70 and nota < 80:
    print("nota: C")

elif nota >= 60 and nota < 70:
    print("nota: D")

else:
    print("nota: F")
```
Introduce una nota: 95  
nota: A  

```python
# Conversión de notas académicas.
nota = int(input("Introduce una nota: "))

if nota >= 90:
    print("nota: A")
elif nota >= 80:
    print("nota: B")
elif nota >= 70:
    print("nota: C")
elif nota >= 60:
    print("nota: D")
else:
    print("nota: F")
```
Sol:  
Introduce una nota: 85  
nota: B  

```python
#Comprobar si un número es par o impar:
valor = int(input("Introduce un número: "))

if valor % 2 == 0:
    print("es par!")

else:
    print("es impar!")
```
Sol:  
Introduce un número: *2*  
es par!  

```python
# Definimos nuestra función: comprobar si un número es par o impar.
def main():
    x = int(input ("Introduce un número: "))
    if es_par(x):
        print("es par!")
    else:
        print("es impar!")

# Creamos una función que realizará el cálculo matemático.
def es_par(n):
    if n % 2 == 0:
        return True
    else:
        return False

# Llamamos a la función.
main()
```
Introduce un número: *6*  
es par!  

```python
# Definimos nuestra función: comprobar si un número es par o impar.
def main():
    x = int(input ("Introduce un número: "))
    if es_par(x):
        print("es par!")
    else:
        print("es impar!")

def es_par(n):
    return True if n % 2 == 0 else False
main()
```
Sol:  
Introduce un número: *8*  
es par!  


La función ***match()*** en Python se utiliza para *realizar una coincidencia entre una expresión y un objeto*. La expresión puede ser una cadena de caracteres, un número, una expresión regular o una función.  

La función ***match()*** devuelve un objeto Match si la coincidencia es exitosa. El objeto Match contiene información sobre la coincidencia, como la posición de la coincidencia y el valor del objeto coincidente.  

```python
# Personajes de Harry Potter.
 name = input ("Introduce tu nmbre: ")

match name:
 case "Harry":
   print("Griffindor")
 case "Hermione":
   print("Griffindor")
 case "Ron":
   print("Griffindor")
 case "Draco":
   print("Slytherin")
 case _:
   print("Who?")
```
Introduce tu nmbre: *Harry*  
Griffindor  

```python
# Personajes de Harry Potter.
name = input ("Introduce tu nmbre: ")

match name:
 case "Harry"| "Hermione" | "Ron":
   print("Griffindor")
 case "Draco":
   print("Slytherin")
 case _:
   print("Who?")
```
Sol:  
Introduce tu nmbre: *Hermione*  
Griffindor 
