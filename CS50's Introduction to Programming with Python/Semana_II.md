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
