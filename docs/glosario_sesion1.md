# 📖 Glosario de Términos - Sesión 1: Fundamentos de Python

Este glosario contiene definiciones de términos técnicos y conceptos de programación que se utilizan en la **Sesión 1** del taller. Está diseñado para que puedas consultarlo después de la sesión y familiarizarte con el vocabulario fundamental de Python.

---

## 📌 Índice por Categoría

- [Conceptos Fundamentales](#conceptos-fundamentales)
- [Variables y Tipos de Datos](#variables-y-tipos-de-datos)
- [Operadores](#operadores)
- [Estructuras de Control](#estructuras-de-control)
- [Funciones](#funciones)
- [Estructuras de Datos](#estructuras-de-datos)
- [Errores y Excepciones](#errores-y-excepciones)
- [Términos Generales](#términos-generales)

---

## Conceptos Fundamentales

### Algoritmo

**Definición:** Serie de pasos ordenados y finitos para resolver un problema o realizar una tarea.

**Ejemplo en la vida real:** Una receta de cocina es un algoritmo (sigue pasos específicos para obtener un resultado).

**Ejemplo en Python:**

```python
# Algoritmo para calcular el promedio de dos números
numero1 = 10
numero2 = 20
suma = numero1 + numero2
promedio = suma / 2
print(promedio)  # 15.0
```

---

### Código Fuente

**Definición:** Texto escrito en un lenguaje de programación que contiene las instrucciones del programa.

**En otras palabras:** Es lo que escribes en el editor (las líneas de Python que ves en tus notebooks).

---

### Comentario

**Definición:** Texto en el código que Python ignora, usado para explicar o documentar el código.

**Símbolo:** Se usa `#` para comentarios de una línea.

**Ejemplo:**

```python
# Este es un comentario
edad = 25  # Comentario al final de una línea
```

**Por qué es importante:** Ayuda a otros (y a ti mismo en el futuro) a entender qué hace tu código.

---

### Ejecutar / Correr

**Definición:** Acción de hacer que Python lea y realice las instrucciones de tu código.

**Sinónimos:** Run, ejecutar, correr el código.

**Ejemplo:** Cuando presionas "Run" en un notebook o ejecutas `python archivo.py` en la terminal.

---

### Indentación

**Definición:** Espacios al inicio de una línea de código que indican el nivel de anidamiento o agrupación.

**Importante:** En Python, la indentación NO es opcional, es parte de la sintaxis.

**Ejemplo:**

```python
if edad >= 18:
    print("Eres mayor de edad")  # Esta línea está indentada
    print("Puedes votar")         # Esta también
print("Fin del programa")         # Esta no está indentada
```

**Regla:** Usa 4 espacios (o una tabulación) para indentar.

---

### Intérprete

**Definición:** Programa que lee y ejecuta código Python línea por línea.

**En otras palabras:** Es el "motor" que hace funcionar Python. Convierte tu código en acciones que la computadora puede realizar.

---

### Sintaxis

**Definición:** Reglas que definen cómo debe escribirse el código en un lenguaje de programación.

**Analogía:** Como las reglas gramaticales en español (sujeto + verbo + predicado).

**Ejemplo correcto:** `print("Hola")`

**Ejemplo incorrecto:** `print "Hola"` (falta paréntesis)

---

## Variables y Tipos de Datos

### Variable

**Definición:** Nombre que se le asigna a un espacio en memoria donde se guarda un valor.

**Analogía:** Como una caja con una etiqueta donde guardas algo.

**Ejemplo:**

```python
nombre = "Ana"      # Variable que guarda texto
edad = 25           # Variable que guarda un número
es_estudiante = True  # Variable que guarda verdadero/falso
```

**Reglas para nombres:**

- Pueden contener letras, números y guion bajo `_`
- No pueden empezar con número
- No pueden usar palabras reservadas de Python
- Son sensibles a mayúsculas (`edad` ≠ `Edad`)

---

### Asignación

**Definición:** Acción de guardar un valor en una variable usando el símbolo `=`.

**Ejemplo:**

```python
x = 10  # Asignamos el valor 10 a la variable x
```

**Nota:** El `=` NO significa "igual que" matemáticamente, significa "asigna el valor".

---

### Tipo de Dato (Data Type)

**Definición:** Categoría que define qué clase de valor contiene una variable y qué operaciones se pueden hacer con ella.

**Tipos básicos en Python:**

- `int` - Números enteros
- `float` - Números decimales
- `str` - Cadenas de texto
- `bool` - Valores booleanos (True/False)

---

### Integer (int)

**Definición:** Tipo de dato para números enteros (sin decimales).

**Ejemplos:**

```python
edad = 25
temperatura = -5
año = 2024
```

---

### Float

**Definición:** Tipo de dato para números con decimales (punto flotante).

**Ejemplos:**

```python
precio = 19.99
temperatura = 36.5
pi = 3.14159
```

**Nota:** En Python se usa punto `.` para decimales, no coma.

---

### String (str)

**Definición:** Tipo de dato para cadenas de texto. Se escriben entre comillas simples `'...'` o dobles `"..."`.

**Ejemplos:**

```python
nombre = "María"
apellido = 'González'
mensaje = "Hola, ¿cómo estás?"
```

**Operaciones comunes:**

```python
texto = "Hola"
len(texto)           # 4 (longitud)
texto.upper()        # "HOLA"
texto.lower()        # "hola"
texto + " Mundo"     # "Hola Mundo" (concatenación)
```

---

### Boolean (bool)

**Definición:** Tipo de dato que solo puede ser `True` (verdadero) o `False` (falso).

**Uso común:** En condiciones y decisiones.

**Ejemplos:**

```python
es_mayor = True
tiene_descuento = False

if es_mayor:
    print("Puede pasar")
```

---

### Conversión de Tipos (Type Casting)

**Definición:** Transformar un valor de un tipo de dato a otro.

**Funciones:**

- `int()` - Convierte a entero
- `float()` - Convierte a decimal
- `str()` - Convierte a texto
- `bool()` - Convierte a booleano

**Ejemplos:**

```python
edad_texto = "25"
edad_numero = int(edad_texto)  # Convierte "25" a 25

precio = 19.99
precio_entero = int(precio)    # Convierte 19.99 a 19

numero = 42
numero_texto = str(numero)     # Convierte 42 a "42"
```

---

## Operadores

### Operador

**Definición:** Símbolo que indica una operación a realizar entre uno o más valores.

---

### Operadores Aritméticos

**Definición:** Operadores para realizar cálculos matemáticos.

| Operador | Nombre | Ejemplo | Resultado |
|----------|--------|---------|-----------|
| `+` | Suma | `5 + 3` | `8` |
| `-` | Resta | `5 - 3` | `2` |
| `*` | Multiplicación | `5 * 3` | `15` |
| `/` | División | `10 / 3` | `3.333...` |
| `//` | División entera | `10 // 3` | `3` |
| `%` | Módulo (residuo) | `10 % 3` | `1` |
| `**` | Potencia | `2 ** 3` | `8` |

---

### Operadores de Comparación

**Definición:** Operadores que comparan dos valores y devuelven `True` o `False`.

| Operador | Significado | Ejemplo | Resultado |
|----------|-------------|---------|-----------|
| `==` | Igual a | `5 == 5` | `True` |
| `!=` | Diferente de | `5 != 3` | `True` |
| `>` | Mayor que | `5 > 3` | `True` |
| `<` | Menor que | `3 < 5` | `True` |
| `>=` | Mayor o igual | `5 >= 5` | `True` |
| `<=` | Menor o igual | `3 <= 5` | `True` |

**Importante:** `==` (doble igual) compara valores. `=` (un solo igual) asigna valores.

---

### Operadores Lógicos

**Definición:** Operadores que combinan o modifican valores booleanos.

| Operador | Significado | Ejemplo | Resultado |
|----------|-------------|---------|-----------|
| `and` | Y lógico | `True and False` | `False` |
| `or` | O lógico | `True or False` | `True` |
| `not` | Negación | `not True` | `False` |

**Ejemplos de uso:**

```python
edad = 20
tiene_permiso = True

# Puede entrar si es mayor de 18 Y tiene permiso
puede_entrar = edad >= 18 and tiene_permiso

# Puede pagar con efectivo O con tarjeta
metodo = "efectivo"
puede_pagar = metodo == "efectivo" or metodo == "tarjeta"
```

---

### Módulo (%)

**Definición:** Operador que devuelve el residuo de una división.

**Uso común:** Determinar si un número es par o impar.

**Ejemplos:**

```python
10 % 2  # 0 (10 dividido entre 2 da residuo 0)
10 % 3  # 1 (10 dividido entre 3 da residuo 1)
15 % 4  # 3 (15 dividido entre 4 da residuo 3)

# Verificar si un número es par
numero = 8
if numero % 2 == 0:
    print("Es par")
```

---

## Estructuras de Control

### Condicional (if/elif/else)

**Definición:** Estructura que permite ejecutar código diferente según se cumplan ciertas condiciones.

**Sintaxis:**

```python
if condicion:
    # Código si la condición es verdadera
elif otra_condicion:
    # Código si la segunda condición es verdadera
else:
    # Código si ninguna condición es verdadera
```

**Ejemplo:**

```python
edad = 20

if edad < 18:
    print("Menor de edad")
elif edad == 18:
    print("Tienes exactamente 18")
else:
    print("Mayor de edad")
```

---

### Ciclo (Loop)

**Definición:** Estructura que repite un bloque de código múltiples veces.

**Tipos principales:**

- `for` - Repite un número conocido de veces
- `while` - Repite mientras una condición sea verdadera

---

### Ciclo for

**Definición:** Repite código para cada elemento de una secuencia.

**Uso común:** Cuando sabes cuántas veces quieres repetir algo.

**Ejemplos:**

```python
# Iterar sobre un rango de números
for i in range(5):
    print(i)  # Imprime 0, 1, 2, 3, 4

# Iterar sobre una lista
frutas = ["manzana", "banana", "naranja"]
for fruta in frutas:
    print(fruta)
```

---

### Ciclo while

**Definición:** Repite código mientras una condición sea verdadera.

**Uso común:** Cuando no sabes cuántas veces se repetirá el ciclo.

**Ejemplo:**

```python
contador = 0
while contador < 5:
    print(contador)
    contador += 1
```

**Cuidado:** Si la condición nunca se vuelve falsa, tendrás un ciclo infinito.

---

### Iteración

**Definición:** Una repetición o vuelta de un ciclo.

**Ejemplo:** Si un ciclo se repite 5 veces, hay 5 iteraciones.

---

### range()

**Definición:** Función que genera una secuencia de números.

**Sintaxis:**

- `range(n)` - Genera números de 0 a n-1
- `range(inicio, fin)` - Genera números desde inicio hasta fin-1
- `range(inicio, fin, paso)` - Genera números con un paso específico

**Ejemplos:**

```python
range(5)           # 0, 1, 2, 3, 4
range(1, 6)        # 1, 2, 3, 4, 5
range(0, 10, 2)    # 0, 2, 4, 6, 8
range(10, 0, -1)   # 10, 9, 8, 7, 6, 5, 4, 3, 2, 1
```

---

### break

**Definición:** Palabra clave que termina un ciclo inmediatamente.

**Ejemplo:**

```python
for i in range(10):
    if i == 5:
        break  # Sale del ciclo cuando i es 5
    print(i)  # Imprime 0, 1, 2, 3, 4
```

---

### continue

**Definición:** Palabra clave que salta a la siguiente iteración del ciclo.

**Ejemplo:**

```python
for i in range(5):
    if i == 2:
        continue  # Salta cuando i es 2
    print(i)  # Imprime 0, 1, 3, 4 (se salta el 2)
```

---

## Funciones

### Función

**Definición:** Bloque de código reutilizable que realiza una tarea específica.

**Analogía:** Como una receta que puedes usar cada vez que necesites cocinar ese platillo.

**Ventajas:**

- Evita repetir código
- Hace el código más organizado
- Facilita encontrar y corregir errores

---

### Definir una Función (def)

**Definición:** Crear una función usando la palabra clave `def`.

**Sintaxis:**

```python
def nombre_funcion(parametros):
    # Código de la función
    return resultado
```

**Ejemplo:**

```python
def saludar(nombre):
    mensaje = f"Hola, {nombre}!"
    return mensaje

# Usar la función
saludo = saludar("Ana")
print(saludo)  # "Hola, Ana!"
```

---

### Parámetro

**Definición:** Variable que recibe valores cuando se llama a una función.

**Ejemplo:**

```python
def sumar(a, b):  # 'a' y 'b' son parámetros
    return a + b

resultado = sumar(5, 3)  # 5 y 3 son argumentos
```

---

### Argumento

**Definición:** Valor real que se pasa a una función cuando se llama.

**Diferencia con parámetro:**

- **Parámetro:** Variable en la definición de la función
- **Argumento:** Valor que se pasa al llamar la función

---

### return

**Definición:** Palabra clave que devuelve un valor desde una función y termina su ejecución.

**Ejemplo:**

```python
def multiplicar(x, y):
    resultado = x * y
    return resultado  # Devuelve el resultado

producto = multiplicar(4, 5)
print(producto)  # 20
```

**Nota:** Si una función no tiene `return`, devuelve `None` por defecto.

---

### Parámetro por Defecto

**Definición:** Valor predefinido para un parámetro que se usa si no se proporciona un argumento.

**Ejemplo:**

```python
def saludar(nombre, saludo="Hola"):
    return f"{saludo}, {nombre}!"

print(saludar("Ana"))              # "Hola, Ana!"
print(saludar("Ana", "Buenos días"))  # "Buenos días, Ana!"
```

---

### Scope (Ámbito)

**Definición:** Región del código donde una variable es accesible.

**Tipos:**

- **Local:** Variables definidas dentro de una función
- **Global:** Variables definidas fuera de todas las funciones

**Ejemplo:**

```python
x = 10  # Variable global

def funcion():
    y = 5  # Variable local
    print(x)  # Puede acceder a x (global)
    print(y)  # Puede acceder a y (local)

funcion()
print(x)  # Funciona
print(y)  # Error: y no existe fuera de la función
```

---

## Estructuras de Datos

### Lista (List)

**Definición:** Colección ordenada y modificable de elementos.

**Sintaxis:** Se usan corchetes `[]`

**Ejemplos:**

```python
frutas = ["manzana", "banana", "naranja"]
numeros = [1, 2, 3, 4, 5]
mixta = [1, "dos", 3.0, True]  # Puede tener tipos diferentes
```

**Operaciones comunes:**

```python
frutas[0]           # Acceder al primer elemento: "manzana"
frutas.append("uva")  # Agregar al final
len(frutas)         # Cantidad de elementos
frutas[1] = "pera"  # Modificar un elemento
```

---

### Índice (Index)

**Definición:** Número que indica la posición de un elemento en una lista o cadena.

**Importante:** En Python, los índices empiezan en 0.

**Ejemplo:**

```python
frutas = ["manzana", "banana", "naranja"]
#          índice 0    índice 1   índice 2

print(frutas[0])  # "manzana"
print(frutas[1])  # "banana"
print(frutas[-1]) # "naranja" (índice negativo: desde el final)
```

---

### Cadena (String)

**Definición:** Secuencia de caracteres (texto).

**Nota:** Las cadenas son inmutables (no se pueden modificar después de crearse).

**Operaciones:**

```python
texto = "Python"
texto[0]          # 'P' (acceder a un carácter)
texto.lower()     # "python"
texto.upper()     # "PYTHON"
texto.replace("P", "J")  # "Jython"
"on" in texto     # True (verifica si contiene "on")
```

---

### Inmutable

**Definición:** Objeto que no puede cambiar después de ser creado.

**Tipos inmutables en Python:** `int`, `float`, `str`, `bool`, `tuple`

**Ejemplo:**

```python
texto = "Hola"
# No puedes hacer: texto[0] = "h"  # Esto da error
# Tienes que crear un nuevo string:
texto = "hola"  # Reasignamos la variable
```

---

### Mutable

**Definición:** Objeto que puede cambiar después de ser creado.

**Tipos mutables en Python:** `list`, `dict`, `set`

**Ejemplo:**

```python
numeros = [1, 2, 3]
numeros[0] = 10  # Funciona, las listas son mutables
print(numeros)   # [10, 2, 3]
```

---

## Errores y Excepciones

### Error (Bug)

**Definición:** Problema en el código que impide que funcione correctamente.

**Tipos comunes:**

- Error de sintaxis (código mal escrito)
- Error de lógica (código hace algo diferente a lo esperado)
- Error de ejecución (código falla al ejecutarse)

---

### Excepción (Exception)

**Definición:** Error que ocurre durante la ejecución del programa.

**Ejemplos comunes:**

```python
# ValueError: tipo de dato incorrecto
int("hola")  # No se puede convertir "hola" a número

# ZeroDivisionError: división por cero
10 / 0

# TypeError: operación entre tipos incompatibles
"5" + 5  # No se puede sumar texto con número

# NameError: variable no definida
print(variable_inexistente)

# IndexError: índice fuera de rango
lista = [1, 2, 3]
print(lista[10])  # No existe el índice 10
```

---

### try-except

**Definición:** Estructura para manejar errores sin que el programa se detenga.

**Sintaxis:**

```python
try:
    # Código que puede causar error
except TipoDeError:
    # Qué hacer si ocurre el error
```

**Ejemplo:**

```python
try:
    edad = int(input("Ingresa tu edad: "))
    print(f"Tienes {edad} años")
except ValueError:
    print("Error: Debes ingresar un número")
```

---

### SyntaxError

**Definición:** Error que ocurre cuando el código no sigue las reglas de sintaxis de Python.

**Ejemplos:**

```python
# Falta dos puntos
if x > 5
    print("Mayor")

# Paréntesis no cerrado
print("Hola"

# Indentación incorrecta
def funcion():
print("Error")  # Falta indentación
```

---

## Términos Generales

### Built-in Function (Función Integrada)

**Definición:** Función que viene incluida en Python, lista para usar sin importar nada.

**Ejemplos comunes:**

- `print()` - Imprime en pantalla
- `input()` - Recibe entrada del usuario
- `len()` - Devuelve la longitud
- `type()` - Devuelve el tipo de dato
- `int()`, `float()`, `str()` - Conversión de tipos
- `range()` - Genera secuencia de números
- `sum()` - Suma elementos de una lista
- `max()`, `min()` - Mayor y menor valor

---

### Método (Method)

**Definición:** Función asociada a un objeto específico.

**Diferencia con función:** Los métodos se llaman con punto `.`

**Ejemplos:**

```python
texto = "hola"
texto.upper()      # upper() es un método de strings

lista = [1, 2, 3]
lista.append(4)    # append() es un método de listas
```

---

### Input/Output (Entrada/Salida)

**Definición:**

- **Input (Entrada):** Datos que el usuario proporciona al programa
- **Output (Salida):** Datos que el programa muestra al usuario

**Funciones:**

```python
nombre = input("¿Cómo te llamas? ")  # Entrada
print(f"Hola, {nombre}")             # Salida
```

---

### print()

**Definición:** Función que muestra texto o valores en la pantalla.

**Ejemplos:**

```python
print("Hola Mundo")
print(42)
print("Tienes", 25, "años")
print(f"Resultado: {5 + 3}")  # Con f-string
```

---

### input()

**Definición:** Función que pide datos al usuario y los devuelve como texto.

**Importante:** `input()` SIEMPRE devuelve un string, aunque el usuario escriba números.

**Ejemplo:**

```python
nombre = input("Tu nombre: ")
edad = int(input("Tu edad: "))  # Convertir a número
```

---

### f-string (Formatted String)

**Definición:** Forma moderna de formatear strings en Python usando `f""`.

**Sintaxis:** Se pone `f` antes de las comillas y se usan `{}` para insertar variables.

**Ejemplos:**

```python
nombre = "Ana"
edad = 25

# f-string
print(f"Me llamo {nombre} y tengo {edad} años")

# Operaciones dentro de {}
print(f"El doble de {edad} es {edad * 2}")

# Formato de decimales
precio = 19.99
print(f"Precio: ${precio:.2f}")  # $19.99 (2 decimales)
```

---

### Concatenación

**Definición:** Unir cadenas de texto usando el operador `+`.

**Ejemplo:**

```python
nombre = "Ana"
apellido = "García"
nombre_completo = nombre + " " + apellido  # "Ana García"

# Alternativa moderna: f-string
nombre_completo = f"{nombre} {apellido}"
```

---

### Expresión

**Definición:** Combinación de valores, variables y operadores que produce un resultado.

**Ejemplos:**

```python
5 + 3           # Expresión que evalúa a 8
x * 2 + 1       # Expresión con variables
edad >= 18      # Expresión booleana (True o False)
```

---

### Instrucción (Statement)

**Definición:** Línea de código que realiza una acción.

**Ejemplos:**

```python
x = 10              # Instrucción de asignación
print("Hola")       # Instrucción de impresión
if x > 5:           # Instrucción condicional
    print("Mayor")
```

---

### Debugging (Depuración)

**Definición:** Proceso de encontrar y corregir errores en el código.

**Técnicas básicas:**

- Usar `print()` para ver valores de variables
- Leer mensajes de error cuidadosamente
- Ejecutar el código línea por línea
- Verificar la lógica del algoritmo

---

### Pythonic

**Definición:** Código que sigue las mejores prácticas y el estilo recomendado de Python.

**Ejemplo no pythonic:**

```python
i = 0
while i < len(lista):
    print(lista[i])
    i += 1
```

**Ejemplo pythonic:**

```python
for elemento in lista:
    print(elemento)
```

---

### PEP 8

**Definición:** Guía de estilo oficial de Python que recomienda cómo escribir código legible.

**Algunas reglas:**

- Usar 4 espacios para indentación
- Nombres de variables en minúsculas con guiones bajos: `mi_variable`
- Nombres de funciones igual: `calcular_promedio()`
- Dejar 2 líneas en blanco antes de definir funciones
- Líneas de máximo 79 caracteres

---

### IDE (Integrated Development Environment)

**Definición:** Programa que facilita escribir, ejecutar y depurar código.

**Ejemplos:** VS Code, PyCharm, Jupyter Notebook

**Características comunes:**

- Editor de código con colores
- Autocompletado
- Detección de errores
- Ejecución de código

---

### Notebook (Jupyter Notebook)

**Definición:** Documento interactivo que combina código, texto y resultados.

**Características:**

- Organizado en celdas (código o markdown)
- Se puede ejecutar celda por celda
- Muestra resultados inmediatamente
- Ideal para aprendizaje y experimentación

---

## 💡 Consejos para Usar este Glosario

1. **No memorices todo:** Este glosario es para consulta, no para memorizar.
2. **Consulta cuando lo necesites:** Si encuentras un término que no entiendes, búscalo aquí.
3. **Practica los ejemplos:** Escribe y ejecuta los ejemplos en tu propio notebook.
4. **Agrega tus notas:** Anota tus propios ejemplos o explicaciones.
5. **Revísalo periódicamente:** Con el tiempo, estos términos se volverán naturales.

---

**📘 Parte de:** Python Essentials - Session 1: Fundamentos de Python

**📅 Última actualización:** Noviembre 2025

**📚 Ver también:** [Recursos Adicionales](recursos_adicionales.md)
