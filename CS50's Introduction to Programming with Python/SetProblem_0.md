## Problema 1: Voz interior.
Implementar un programa en Python que solicite al usuario una entrada y luego genere esa misma entrada en minúsculas.

```python
# Creamos una variable que almacenará la información generada por el usuario:
mensaje = input("Introduce un mensaje: ")

"""
Creamos una nueva variable que almacenará la nueva cadena de texto transformada.
.lower() es una función en Python que transforma cualquier cadena de texto en minúscula.
"""
mensaje_minuscula = mensaje.lower()

# Salida:
print(mensaje_minuscula)
```
Sol:  
Introduce un mensaje: *HELLO*  
hello  

Introduce un mensaje: *THIS IS CS50*  
this is cs50  

Códigos alternativos:
```python
mensaje = (input("Introduce un mensaje: ")).lower()

print(mensaje)
```
```python
mensaje = input("Introduce un mensaje: ")

print(mensaje.lower())
```

## Problema 2: Velocidad de reproducción.
Implemente un programa en Python que solicite al usuario una entrada y luego genere esa misma entrada, reemplazando cada espacio con ...(es decir, tres puntos).

```python
# Creamos una variable que contenga el mensaje introducido por el usuario:
mensaje = input("Introduce un mensaje: ")

"""
Creamos una nueva variable que contenga el mensaje formateado.
Utilizamos el método .replace() para reemplazar el espacio en blanco por ... (3 puntos) entre las cadenas de caracteres.
"""
mensaje_nuevo = mensaje.replace(" ", "...")

# Salida del mensaje:
print(mensaje_nuevo)
```
Sol:  
Introduce un mensaje: *This is CS50*  
*This...is...CS50*
