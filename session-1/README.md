# Sesión 1 — Fundamentos de Python

## 🎯 Objetivo de la Sesión

Esta sesión introduce los fundamentos de la programación con Python desde cero. Al finalizar, los participantes podrán:

- Comprender los conceptos básicos de programación
- Escribir y ejecutar programas simples en Python
- Utilizar variables, tipos de datos y operadores
- Implementar lógica con condicionales y ciclos
- Crear y utilizar funciones para organizar código
- Desarrollar un mini proyecto funcional

**No se requiere experiencia previa en programación.** Todo se explica desde el principio.

---

## 📚 Temario Detallado

### 1. Variables y Asignación
- ¿Qué es una variable?
- Nombres de variables y convenciones
- Asignación y reasignación de valores
- Impresión en consola con `print()`

### 2. Tipos de Datos
- Números: `int` y `float`
- Cadenas de texto: `str`
- Booleanos: `bool`
- Conversión entre tipos
- Operaciones básicas con cada tipo

### 3. Estructuras de Control: Condicionales
- Expresiones booleanas
- Operadores de comparación (`==`, `!=`, `<`, `>`, `<=`, `>=`)
- Estructura `if`, `elif`, `else`
- Operadores lógicos (`and`, `or`, `not`)
- Condicionales anidados

### 4. Estructuras de Control: Ciclos
- El ciclo `for`: iteración sobre secuencias
- El ciclo `while`: iteración condicional
- `range()` para generar secuencias numéricas
- `break` y `continue`
- Listas básicas para iterar

### 5. Funciones
- ¿Por qué usar funciones?
- Definición de funciones con `def`
- Parámetros y argumentos
- Valores de retorno con `return`
- Ámbito de variables (scope)
- Funciones con múltiples parámetros

### 6. Mini Proyecto Integrador
- Aplicación práctica de todos los conceptos
- Desarrollo paso a paso
- Retos opcionales para profundizar

---

## 🗂️ Estructura del Contenido

```
session-1/
├── README.md                           # Este archivo
├── ejemplos/                           # Notebooks con explicaciones y ejemplos
│   ├── variables.ipynb                # Introducción a variables
│   ├── tipos_datos.ipynb              # Tipos de datos en Python
│   ├── condicionales.ipynb            # Estructuras if/elif/else
│   ├── ciclos.ipynb                   # Bucles for y while
│   └── funciones.ipynb                # Definición y uso de funciones
├── ejercicios/                        # Práctica guiada
│   ├── ejercicios_nivel_1.ipynb      # Ejercicios básicos
│   ├── ejercicios_nivel_2.ipynb      # Ejercicios intermedios
│   └── soluciones/                    # Soluciones detalladas
│       ├── soluciones_nivel_1.ipynb
│       └── soluciones_nivel_2.ipynb
└── mini_proyecto/                     # Proyecto integrador
    └── proyecto_basico.ipynb          # Calculadora interactiva
```

---

## 🔗 Relación con el Taller Completo

### Conexión Conceptual

Esta sesión sienta las **bases fundamentales** para todo el taller:

- **Para la Sesión 2 (Datos):** Los conceptos de variables, tipos de datos, ciclos y funciones son esenciales para manipular datos con pandas y numpy. Sin embargo, la Sesión 2 puede tomarse de manera independiente ya que repasa estos conceptos brevemente.

- **Para la Sesión 3 (GenAI):** Las funciones, condicionales y manejo de strings son cruciales para trabajar con APIs de IA. La Sesión 3 también es independiente y repasa lo necesario.

### Independencia de las Sesiones

**Importante:** Aunque los conceptos se relacionan, cada sesión está diseñada para ser independiente. Los participantes pueden unirse a cualquier sesión sin haber asistido a las anteriores. Se hará una revisión rápida de conceptos clave al inicio de cada sesión.

---

## 🚀 Cómo Usar Este Material

### Requisitos Previos

- Python 3.8 o superior instalado
- Visual Studio Code con la extensión de Python
- **No se requieren librerías externas** (solo Python estándar)

### Orden Recomendado

1. **Estudia los ejemplos** (carpeta `ejemplos/`):
   - Ve en orden: variables → tipos_datos → condicionales → ciclos → funciones
   - Ejecuta cada celda y experimenta modificando los valores

2. **Practica con los ejercicios** (carpeta `ejercicios/`):
   - Comienza con `ejercicios_nivel_1.ipynb`
   - Intenta resolver sin ver las soluciones
   - Consulta las soluciones solo después de intentar
   - Continúa con `ejercicios_nivel_2.ipynb`

3. **Desarrolla el mini proyecto** (carpeta `mini_proyecto/`):
   - Sigue las instrucciones paso a paso
   - Intenta completar los retos opcionales
   - Modifica el proyecto para hacerlo tuyo

### Cómo Abrir y Ejecutar los Notebooks

#### Opción 1: Desde VS Code (Recomendado)

1. Abre VS Code
2. Abre la carpeta `session-1` (File → Open Folder)
3. Navega a cualquier notebook (.ipynb)
4. Haz clic en el archivo para abrirlo
5. Selecciona el kernel de Python cuando se solicite
6. Ejecuta las celdas con `Shift + Enter` o el botón ▶️

#### Opción 2: Desde Jupyter Notebook

```bash
# Instala Jupyter si no lo tienes
pip install notebook

# Navega a la carpeta session-1
cd session-1

# Inicia Jupyter Notebook
jupyter notebook
```

#### Opción 3: Desde Jupyter Lab

```bash
# Instala Jupyter Lab si no lo tienes
pip install jupyterlab

# Navega a la carpeta session-1
cd session-1

# Inicia Jupyter Lab
jupyter lab
```

---

## 💡 Consejos para Aprender

1. **Experimenta:** No tengas miedo de modificar el código y ver qué pasa
2. **Practica:** La programación se aprende haciendo, no solo leyendo
3. **Comete errores:** Los errores son parte del aprendizaje
4. **Toma notas:** Agrega tus propias celdas con comentarios
5. **Sé paciente:** Dominar la programación toma tiempo y práctica

---

## 📖 Recursos Adicionales

### Documentación Oficial
- [Tutorial oficial de Python (español)](https://docs.python.org/es/3/tutorial/)
- [Python para principiantes](https://www.python.org/about/gettingstarted/)

### Práctica Extra
- [Ejercicios de Python en línea](https://www.practicepython.org/)
- [Python Tutor](http://pythontutor.com/) - Visualiza cómo se ejecuta tu código

---

## 🆘 Solución de Problemas

### El notebook no se abre
- Verifica que VS Code tenga la extensión de Python instalada
- Intenta instalar Jupyter: `pip install notebook`

### El código no se ejecuta
- Asegúrate de haber seleccionado un kernel de Python
- Verifica que Python esté instalado correctamente: `python --version`

### Error al ejecutar una celda
- Lee el mensaje de error cuidadosamente
- Verifica que hayas ejecutado las celdas anteriores en orden
- Intenta reiniciar el kernel (Restart en el menú)

---

## 🎓 Después de Esta Sesión

Una vez completada esta sesión, tendrás las habilidades para:

✅ Escribir programas básicos en Python  
✅ Entender código Python que encuentres en línea  
✅ Continuar con la Sesión 2 (Análisis de Datos)  
✅ Continuar con la Sesión 3 (GenAI)  
✅ Explorar proyectos personales simples  
✅ Seguir aprendiendo de forma autónoma  

---

## 📞 Contacto y Soporte

Si tienes preguntas durante o después del taller:
- Consulta la documentación en `docs/`
- Revisa las soluciones en `ejercicios/soluciones/`
- Contacta al instructor del taller

---

**¡Disfruta aprendiendo Python! 🐍✨**
