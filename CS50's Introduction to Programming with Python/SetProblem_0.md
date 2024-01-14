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

Código alternativo:
```python
mensaje = input("Introduce un mensaje: ")
print(mensaje.replace(" ", "..."))
```
Sol:  
Introduce un mensaje: *This is CS50*  
*This...is...CS50*  

## Problema 3: Haciendo caras.
Implemente una función llamada ***convert*** que acepte a **str** como entrada y devuelva esa misma entrada con cualquier :) convertido a 🙂 (también conocido como una cara ligeramente sonriente) y cualquier :( convertido a 🙁 (también conocido como una cara ligeramente triste). El resto del texto debe devolverse sin cambios.

Luego, en ese mismo archivo, implemente una función llamada ***main*** que solicita al usuario una entrada, llama ***convert*** a esa entrada e imprime el resultado.

```python
# Función principal:
def main():
    # Creamos una variable con el mensaje de entrada.
    mensaje_usuario = input()
    # Creamos una variable con el valor obtenido de la función de conversión.
    resultado = convert(mensaje_usuario)
    # Salida.
    print(resultado)

# Función de conversión que depende de la variable mensaje_usuario.
def convert(mensaje_usuario):
    # Transformación para la carita feliz:
    caritafeliz = mensaje_usuario.replace(":)", "😀")
    # Transformación para la carita triste:
    caritatriste = caritafeliz.replace(":(", "☹️")
    # Salida del valor de la función:
    return caritatriste

# Llamada de la función.
main()
```
Sol:  
*hello :)*  
*hello* 😀  

Código alternativo:  
```python
def main():
    texto = input()
    textofinal = convert(texto)
    print(textofinal)

def convert(texto):
   carita = texto.replace(":)" , "🙂").replace(":(" , "🙁")
   return carita

main()
```
Sol:  
*hello :(*  
*hello* 🙁  
