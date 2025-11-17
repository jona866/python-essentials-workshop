# Guía de Preparación por Sesión

**Programa:** Python Essentials  Programación, Datos y GenAI

---

## SESIÓN 1 - Python desde Cero: Fundamentos para Programar

Esta sesión no requiere conocimientos previos. Solo necesitas instalar Python y Visual Studio Code.

### 1. Instalar Python

1. Entra a: [https://www.python.org/downloads/](https://www.python.org/downloads/)
2. Descarga la versión más reciente recomendada
3. Ejecuta el instalador
4. **Importante:** Activa la casilla **"Add Python to PATH"**
5. Finaliza la instalación

**Para verificar:**

Abre una terminal y ejecuta:

```bash
python --version
```

### 2. Instalar Visual Studio Code

1. Descarga desde: [https://code.visualstudio.com/](https://code.visualstudio.com/)
2. Instala con las opciones por defecto

### 3. Instalar la extensión de Python en VS Code

1. Abre VS Code
2. Ve a **"Extensiones"** (Ícono de cuadrados en la barra lateral)
3. Busca **Python (Microsoft)**
4. Haz clic en **Install**

### Opcional (pero recomendado)

#### Crear una cuenta de GitHub

- Útil para descargar repositorios y guardar tus avances
- Regístrate en: [https://github.com/](https://github.com/)

#### Instalar Git (opcional)

- Permite clonar repositorios
- Descarga: [https://git-scm.com/downloads](https://git-scm.com/downloads)
- Si no lo instalas, podrás descargar el material como ZIP

### Con esto estás listo para la sesión 1

Todas las librerías, archivos y configuraciones del entorno se harán durante la sesión.

---

## SESIÓN 2 - Python para Datos: Análisis, ETL y Preparación

Si participas en esta sesión, la preparación es prácticamente la misma que en la sesión 1.

### 1. Tener Python y VS Code listos

- La sesión intermedia utiliza exactamente las mismas herramientas base
- No necesitas instalar ninguna librería, estas se configuraron en vivo durante el taller

### 2. Dataset

- El dataset será proporcionado durante la sesión
- Si quieres traer un dataset propio en formato CSV, también podrás usarlo

### Esto es todo

La instalación de librerías, notebooks, scripts y manejo de archivos se hará durante la sesión.

---

## SESIÓN 3 - GenAI con Semantic Kernel y Modelo Local

En esta sesión trabajaremos con modelos de IA que se ejecutan localmente mediante Ollama.  
La instalación es sencilla.

### 1. Tener listo Python y VS Code

Mismo entorno que en las sesiones anteriores.

### 2. Instalar Ollama

1. Entra a: [https://ollama.com](https://ollama.com)
2. Descarga la versión para tu sistema operativo
3. Instálalo con las opciones por defecto
4. Reinicia tu equipo si lo solicita

**Para verificar:**

```bash
ollama --version
```

### 3. Descargar un modelo local

Se recomienda descargar antes del taller uno de estos modelos:

**Modelo recomendado (más ligero):**

```bash
ollama pull phi3
```

**Alternativa más robusta:**

```bash
ollama pull llama3:8b
```

> **Nota:** Esta es la única descarga significativa previa al taller.

### Importante

- **No instales librerías adicionales** y no configures ningún entorno virtual
- Todo se hará durante la sesión mediante archivos proporcionados, incluyendo el `.env`

### Con esto estás listo para la sesión 3

El resto de configuraciones, instalación de dependencias y estructura del proyecto se resolverán paso a paso durante la clase.

---

## CHECKLIST RESUMIDO

### General (todas las sesiones)

- [ ] Python instalado
- [ ] Visual Studio Code instalado
- [ ] Extensión de Python instalada en VS Code
- [ ] Cuenta de GitHub creada (opcional)
- [ ] Git instalado (opcional, se puede usar ZIP)

### Sesión 1 - Fundamentos

- [ ] Python listo
- [ ] VS Code listo
- [ ] Sin instalación de librerías

### Sesión 2 - Datos

- [ ] Todo lo de la sesión 1
- [ ] Dataset listo (si deseas usar uno propio)
- [ ] Las librerías se instalaron en la sesión

### Sesión 3 - GenAI

- [ ] Python y VS Code listos
- [ ] Ollama instalado
- [ ] Modelo descargado (phi3 recomendado)
- [ ] Sin librerías ni entorno configurado (se hará en taller)
