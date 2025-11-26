# 🎮 Mini Proyecto: Calculadora Interactiva

## 📋 Descripción del Proyecto

En este proyecto vas a crear una **calculadora interactiva** que funcione desde la terminal. El proyecto te permitirá aplicar todos los conceptos aprendidos en la Sesión 1.

---

## 🎯 Objetivos

Al completar este proyecto, habrás aplicado:
- ✅ Variables y tipos de datos
- ✅ Condicionales (if/elif/else)
- ✅ Ciclos (while, for)
- ✅ Funciones
- ✅ Listas
- ✅ Entrada y salida de datos
- ✅ Validación de errores

---

## 📝 Requisitos del Proyecto

Tu calculadora debe tener las siguientes características:

### 1. Operaciones Básicas
- Sumar dos números
- Restar dos números
- Multiplicar dos números
- Dividir dos números (con validación de división por cero)

### 2. Operaciones Avanzadas
- Calcular potencia (base^exponente)
- Calcular raíz cuadrada
- Calcular porcentaje de un número
- Calcular módulo (residuo de división)

### 3. Funcionalidades Adicionales
- Menú interactivo que muestre todas las opciones
- Opción para salir del programa
- Historial de operaciones realizadas
- Validación de entradas del usuario

---

## 🏗️ Estructura Sugerida

### Paso 1: Crear las Funciones Matemáticas Básicas

Crea funciones para cada operación básica:

```python
def sumar(a, b):
    # Tu código aquí
    pass

def restar(a, b):
    # Tu código aquí
    pass

def multiplicar(a, b):
    # Tu código aquí
    pass

def dividir(a, b):
    # Tu código aquí
    # Recuerda validar que b no sea cero
    pass
```

**Consejo:** Prueba cada función con valores de ejemplo para verificar que funcionen correctamente.

---

### Paso 2: Crear las Funciones Matemáticas Avanzadas

Agrega funciones para operaciones más complejas:

```python
def potencia(base, exponente):
    # Tu código aquí
    pass

def raiz_cuadrada(numero):
    # Tu código aquí
    # Recuerda validar que el número no sea negativo
    pass

def calcular_porcentaje(cantidad, porcentaje):
    # Tu código aquí
    pass

def modulo(a, b):
    # Tu código aquí
    pass
```

---

### Paso 3: Crear la Función del Menú

Crea una función que muestre las opciones disponibles:

```python
def mostrar_menu():
    print("\n" + "="*50)
    print("     CALCULADORA INTERACTIVA")
    print("="*50)
    # Agrega todas las opciones aquí
    # 1. Sumar
    # 2. Restar
    # ... etc
```

**Consejo:** Usa emojis y separadores para hacer el menú más atractivo visualmente.

---

### Paso 4: Crear Función de Validación de Entrada

Esta función debe pedir un número al usuario y validar que la entrada sea correcta:

```python
def obtener_numero(mensaje):
    while True:
        try:
            numero = float(input(mensaje))
            return numero
        except ValueError:
            print("Error: Por favor ingresa un número válido")
```

**Nota:** Esta función usa `try-except` para manejar errores. Si el usuario ingresa texto en lugar de un número, se le pedirá que intente nuevamente.

---

### Paso 5: Crear la Función Principal

Esta es la función más importante. Debe:

1. Crear una lista vacía para el historial
2. Mostrar un mensaje de bienvenida
3. Entrar en un ciclo while que:
   - Muestre el menú
   - Pida al usuario que seleccione una opción
   - Ejecute la operación correspondiente
   - Guarde el resultado en el historial
   - Permita al usuario continuar o salir

```python
def calculadora():
    historial = []  # Lista para guardar operaciones
    
    print("¡Bienvenido a la Calculadora Interactiva!")
    
    while True:
        mostrar_menu()
        opcion = input("Selecciona una opción: ")
        
        # Aquí va tu lógica para manejar cada opción
        
        if opcion == "0":  # Opción para salir
            print("¡Gracias por usar la calculadora!")
            # Mostrar historial antes de salir
            break
```

**Estructura del ciclo principal:**

- Si el usuario elige opción 1 (Sumar):
  - Pedir dos números
  - Llamar a la función `sumar()`
  - Mostrar el resultado
  - Guardar en historial

- Repetir para todas las opciones

- Si el usuario elige ver historial:
  - Recorrer la lista de historial
  - Mostrar cada operación

---

## 📊 Ejemplo de Funcionamiento

```
==================================================
     🧮 CALCULADORA INTERACTIVA 🧮
==================================================

📊 Operaciones Básicas:
  1. Sumar
  2. Restar
  3. Multiplicar
  4. Dividir

🔢 Operaciones Avanzadas:
  5. Potencia
  6. Raíz cuadrada
  7. Calcular porcentaje
  8. Módulo

📜 Otras Opciones:
  9. Ver historial
  0. Salir

==================================================

👉 Selecciona una opción: 1

📝 Ingresa los números:
  Primer número: 25
  Segundo número: 17

✅ Resultado: 25 + 17 = 42

Presiona Enter para continuar...
```

---

## 🎯 Checklist de Funcionalidades

Usa esta lista para verificar que tu proyecto está completo:

### Funciones Básicas
- [ ] Función `sumar(a, b)`
- [ ] Función `restar(a, b)`
- [ ] Función `multiplicar(a, b)`
- [ ] Función `dividir(a, b)` con validación de división por cero

### Funciones Avanzadas
- [ ] Función `potencia(base, exponente)`
- [ ] Función `raiz_cuadrada(numero)` con validación de número negativo
- [ ] Función `calcular_porcentaje(cantidad, porcentaje)`
- [ ] Función `modulo(a, b)`

### Sistema de Menú
- [ ] Función `mostrar_menu()` que muestra todas las opciones
- [ ] Menú visualmente organizado y claro

### Validación
- [ ] Función `obtener_numero(mensaje)` que valida entradas
- [ ] Manejo de errores con try-except

### Funcionalidad Principal
- [ ] Función `calculadora()` que coordina todo
- [ ] Ciclo while que mantiene el programa corriendo
- [ ] Lista para guardar historial de operaciones
- [ ] Opción para ver historial
- [ ] Opción para salir del programa
- [ ] Al salir, muestra el historial completo

### Extras (Opcional)
- [ ] Mensajes con emojis
- [ ] Formato de números con decimales limitados
- [ ] Pausas para que el usuario lea resultados
- [ ] Manejo de opciones inválidas

---

## 🚀 Retos Opcionales

Si terminas el proyecto básico y quieres ir más allá, intenta estos retos:

### Reto 1: Agregar Más Operaciones
- Factorial de un número
- Secuencia de Fibonacci
- Conversión de temperatura (Celsius ↔ Fahrenheit)

### Reto 2: Mejorar el Historial
- Opción para limpiar el historial
- Guardar el historial en un archivo de texto
- Mostrar fecha y hora de cada operación

### Reto 3: Calculadora Científica
- Funciones trigonométricas (necesitarás importar `math`)
- Logaritmos
- Valor absoluto

### Reto 4: Conversiones
- Conversor de monedas
- Conversor de unidades (metros, kilómetros, millas)
- Conversor de peso

---

## 💡 Consejos y Tips

### Para Empezar
1. **No intentes hacer todo a la vez.** Empieza por las funciones básicas y pruébalas.
2. **Usa comentarios** para explicar tu código.
3. **Prueba cada función** individualmente antes de integrarla al menú.

### Para Depurar (Debug)
1. **Usa print()** para ver qué valores tienen tus variables.
2. **Prueba con casos extremos:** números negativos, cero, números muy grandes.
3. **Lee los mensajes de error** cuidadosamente, te dicen dónde está el problema.

### Para Organizar
1. **Agrupa las funciones relacionadas** juntas.
2. **Deja espacios** entre secciones para mejor legibilidad.
3. **Usa nombres descriptivos** para variables y funciones.

---

## ✅ Criterios de Evaluación

Tu proyecto será considerado completo y exitoso si:

1. **Funcionalidad (40%)**
   - Todas las operaciones funcionan correctamente
   - El menú es interactivo y funcional
   - El historial guarda y muestra operaciones

2. **Validación (25%)**
   - Maneja división por cero
   - Valida entradas del usuario
   - Maneja opciones inválidas del menú

3. **Código (20%)**
   - Usa funciones apropiadamente
   - El código está organizado y es legible
   - Tiene comentarios explicativos

4. **Experiencia de Usuario (15%)**
   - El menú es claro y fácil de usar
   - Los mensajes son informativos
   - La calculadora es agradable de usar

---

## 📚 Recursos de Ayuda

Si te atoras, puedes:
1. Revisar los notebooks de ejemplos en la carpeta `ejemplos/`
2. Consultar los ejercicios resueltos en `ejercicios/soluciones/`
3. Buscar en la documentación oficial de Python
4. Pedir ayuda al instructor

---

## 🎉 ¡Manos a la Obra!

Ahora que tienes todas las instrucciones, ¡es hora de crear tu calculadora!

**Recuerda:** Este proyecto es tu oportunidad de aplicar todo lo aprendido. No te preocupes si no sale perfecto al primer intento. La programación es un proceso iterativo de probar, fallar, aprender y mejorar.

**¡Buena suerte y diviértete programando! 🐍✨**
