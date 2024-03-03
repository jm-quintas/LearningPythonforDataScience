# Excepciones.

## Error de Sintaxis.

Los errores de sintaxis en Python se producen cuando el código no está escrito correctamente, lo que impide que el intérprete de Python lo ejecute. Algunos ejemplos comunes de errores de sintaxis son:
* ***Falta de paréntesis:***
```python
print("Hola mundo")  # Correcto
print "Hola mundo")  # Error: Falta un paréntesis después de la función print
```
* ***Comillas no coincidentes:***
```python
print('Hola mundo')  # Correcto
print('Hola mundo")  # Error: Las comillas simples no coinciden con las dobles
```
* ***Errores en la indentación:***
```python
if True:
  print("Hola mundo")
    print("Adios mundo")  # Error: La segunda línea no está indentada correctamente
```
* ***Palabras clave mal escritas:***
```python
if True:
  print("Hola mundo")  # Correcto
If True:
  print("Hola mundo")  # Error: La palabra clave "if" está mal escrita
```

### Para identificar y corregir errores de sintaxis:
* ***Presta atención al mensaje de error:*** El intérprete de Python suele proporcionar un mensaje de error que indica la línea donde se encuentra el error y una breve descripción del problema.
* ***Revisa la indentación:*** Asegúrate de que las líneas de código estén indentadas correctamente, especialmente dentro de bloques condicionales.
* ***Comprueba la sintaxis básica:*** Verifica que los paréntesis, las comillas y los puntos y comas estén correctamente escritos.
* ***Utiliza un editor de código con resaltado de sintaxis:*** Esto te ayudará a identificar errores de sintaxis más fácilmente.
* ***Consulta la documentación de Python:*** La documentación oficial de Python [](https://docs.python.org/3/) ofrece información detallada sobre la sintaxis del lenguaje.

### Consejos para evitar errores de sintaxis:
* ***Escribe el código con cuidado:*** Presta atención a los detalles y asegúrate de que cada línea de código esté escrita correctamente.
* ***Prueba el código a menudo:*** Ejecuta el código con frecuencia para identificar y corregir errores de sintaxis.
* ***Utiliza herramientas de depuración:*** Los IDEs y depuradores pueden ayudarte a identificar y corregir errores de sintaxis más fácilmente.

**Recuerda:** Los errores de sintaxis son errores comunes, especialmente para principiantes. Con práctica y atención a los detalles, podrás escribir código Python con mayor precisión y evitar este tipo de errores.
