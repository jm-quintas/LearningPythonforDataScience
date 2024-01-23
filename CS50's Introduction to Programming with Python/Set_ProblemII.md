## Problema 1: camelCase.
En un archivo llamado camel.py, implemente un programa que solicite al usuario el nombre de una variable en ***camel case*** y genere el nombre correspondiente en ***snake case***. Supongamos que la entrada del usuario será en camel case.  

```python
# Entrada por porte del usuario:
cadena_texto = input("camelCase: ")

# Salida snake_case:
print("snake_case: ", end = "")

# Utilizamos el bucle for para recorrer palabras:
for letra in cadena_texto:
    # Demostración de la iteración
    # print(letra)

    """
    El método .isupper() en Python se utiliza para comprobar 
    si todos los caracteres de una cadena son mayúsculas. 
    Devuelve True si todos los caracteres son mayúsculas y 
    False si hay algún carácter en minúscula.

    El método .lower(), retorna una copia de la cadena de 
    caracteres con todas las letras en minúsculas.
    """

    # Utilizamos los condicionales if y else para comprobar:
    if letra.isupper():
        print("_" + letra.lower(), end = "")

    else:
        print(letra, end = "")
```
Sol:  
camelCase: ***nameFirst***  
snake_case: ***name_first***  

## Problema 2: Máquina de coca-cola.
Implemente un programa que solicite al usuario que inserte una moneda, una a la vez, informándole cada vez el monto adeudado. Una vez que el usuario haya ingresado al menos 50 centavos, indique cuántos centavos de cambio se le deben al usuario. Supongamos que el usuario solo ingresará números enteros e ignorará cualquier número entero que no sea una denominación aceptada.

```Python
# Cantidad a pagar:
monto_adeudado = 50

# Utilizamos el bucle while:
while monto_adeudado > 0:
    # Imprimir la cantidad adeudada:
    print("Amount Due: ", monto_adeudado)

    # Preguntar al usuario que inserte dinero:
    dinero = int(input("Insert coin: "))

    # Comprobar si el dinero es 25, 10 o 5 centavos:
    # Utilizamos una condicional:
    if dinero in [25, 10, 5]:
        # Restar la cantidad adeudada del dinero ingresado:
        monto_adeudado = monto_adeudado - dinero

        # Imprimir la cantidad resultante:
        # print(monto_adeudado)

# Cambio:
cambio = abs(monto_adeudado)
print("Change_Owed:", cambio)
```
Sol:  
Amount Due:  50  
Insert coin: 25  
Amount Due:  25  
Insert coin: 10  
Amount Due:  15  
Insert coin: 25  
Change_Owed: 10  

