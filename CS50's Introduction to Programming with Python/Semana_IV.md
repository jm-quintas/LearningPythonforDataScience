# Excepciones.
Las excepciones son eventos inesperados que interrumpen el flujo normal del programa.

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

## Errores de Valores.
Los errores de valores en Python se producen cuando el intérprete de Python encuentra un valor inesperado durante la ejecución del código. Algunos ejemplos comunes de errores de valores son:
* ***Errores de tipo:***
```python
numero = "10"
suma = numero + 1  # Error: Se intenta sumar un tipo str con un tipo int
```
* ***Errores de índice:***
```python
lista = [1, 2, 3]
valor = lista[5]  # Error: Se intenta acceder a un índice fuera de la lista
```
* ***Errores de nombre:***
```python
variable_no_definida  # Error: Se intenta usar una variable que no está definida
```
* ***Errores de módulo:***
```python
import modulo_no_existente  # Error: Se intenta importar un módulo que no existe
```
* ***Errores de división por cero:***
```python
division = 10 / 0  # Error: Se intenta dividir un número por cero
```
### Para identificar y corregir errores de valores:
* ***Presta atención al mensaje de error:*** El intérprete de Python suele proporcionar un mensaje de error que indica la línea donde se encuentra el error y una breve descripción del problema.
* ***Revisa el tipo de datos:*** Asegúrate de que los tipos de datos de los valores sean compatibles con la operación que se está realizando.
* ***Comprueba los nombres de las variables:*** Verifica que las variables estén correctamente escritas y definidas.
* ***Asegúrate de que los módulos existen:*** Revisa que los módulos que se importan estén instalados y correctamente configurados.
* ***Maneja las excepciones:*** Puedes utilizar bloques try/except para manejar errores de valores específicos.

### Consejos para evitar errores de valores:
* ***Utiliza el tipado estático:*** Puedes declarar el tipo de dato de las variables para evitar errores de tipo.
* ***Valida los valores:*** Puedes utilizar funciones para verificar que los valores sean correctos antes de usarlos.
* ***Documenta tu código:*** Escribir comentarios en tu código te ayudará a comprender mejor el significado de las variables y las operaciones.
* ***Prueba el código a menudo:*** Ejecuta el código con frecuencia para identificar y corregir errores de valores.
* ***Utiliza herramientas de depuración:*** Los IDEs y depuradores pueden ayudarte a identificar y corregir errores de valores más fácilmente.
