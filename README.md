#  Análisis Exploratorio de Datos (EDA) con Python

Material didáctico de **Ciencia de Datos** para estudiantes de **7.º semestre de la carrera de Sistemas**.

A partir de un dataset real de un catálogo de libros (`book1.csv`, 1 000 registros), el estudiante recorre el proceso completo de un EDA: desde entender el problema hasta comunicar hallazgos con sus limitaciones.

---

## 📁 Contenido del repositorio

| Archivo | Descripción | Para quién |
|---------|-------------|------------|
| [`01_EDA_Clase.ipynb`](01_EDA_Clase.ipynb) | Clase completa en formato **presentación**: conceptos básicos y avanzados con ejemplos ejecutados | Docente y estudiantes |
| [`02_EDA_Ejercicios.ipynb`](02_EDA_Ejercicios.ipynb) | 49 ejercicios (100 pts + 3 bonus) con **autoverificación** ✅ / ❌ / ⏳ | Estudiantes |
| [`book1.csv`](book1.csv) | Dataset del caso de estudio | Todos |
| [`requirements.txt`](requirements.txt) | Librerías necesarias | Todos |

---

## 🎯 Objetivos de aprendizaje

Al terminar, el estudiante será capaz de:

1. Formular el **contexto y las preguntas de negocio** que guían un análisis.
2. **Cargar, inspeccionar y describir** un dataset (dimensiones, variables y tipos de datos).
3. **Evaluar la calidad de los datos** y documentar las decisiones de limpieza.


---

## 🗺️ Las 13 etapas del EDA

| # | Etapa | # | Etapa |
|---|-------|---|-------|
| 1 | Contexto del problema | 8 | Calidad de los datos |
| 2 | Conociendo el dataset | 9 | Estadísticas básicas |
| 3 | Cargar los datos | 10 | Agrupaciones |
| 4 | Primer vistazo | 11 | Preguntas de negocio |
| 5 | Dimensiones | 12 | Visualización |
| 6 | Variables | 13 | Interpretación |
| 7 | Tipos de datos | | |


---

## 📦 Dataset

`book1.csv` contiene **1 000 libros** y **7 columnas**:

| Columna | Descripción | Tipo |
|---------|-------------|------|
| `Titulo` | Nombre del libro | Texto |
| `Rating` | Valoración en estrellas (1 a 5) | Ordinal |
| `Precio` | Precio de venta (£ en el sitio original) | Continua |
| `Stock` | Unidades disponibles | Discreta |
| `URL` | Enlace a la ficha del libro | Identificador |
| `Descripcion` | Sinopsis del libro | Texto libre |
| `Categoria` | Género o categoría | Nominal |

> 🧪 **Nota:** los datos fueron obtenidos por *web scraping* de [books.toscrape.com](https://books.toscrape.com), un sitio creado para practicar scraping. Contiene **problemas de calidad reales de captura** que se trabajan en la etapa 8 (por ejemplo, variables constantes, categorías falsas y texto duplicado). Los precios y ratings no representan datos comerciales reales.

---

## 🚀 Cómo ejecutar los notebooks

### Opción A — Google Colab (sin instalar nada)

1. Abre el notebook desde GitHub en Colab:
   `https://colab.research.google.com/github/TU_USUARIO/TU_REPOSITORIO/blob/main/02_EDA_Ejercicios.ipynb`
2. En la **primera celda de código**, cambia la ruta para leer el CSV directo desde GitHub:

   ```python
   RUTA = "https://raw.githubusercontent.com/TU_USUARIO/TU_REPOSITORIO/main/book1.csv"
   ```

   *(Alternativa: sube `book1.csv` al panel de archivos de Colab y deja `RUTA = "book1.csv"`.)*

### Opción B — Instalación local

```bash
# 1. Clonar el repositorio
git clone https://github.com/TU_USUARIO/TU_REPOSITORIO.git
cd TU_REPOSITORIO

# 2. Crear y activar un entorno virtual (recomendado)
python -m venv venv
source venv/bin/activate        # Linux / macOS
venv\Scripts\activate           # Windows

# 3. Instalar dependencias
pip install -r requirements.txt

# 4. Abrir Jupyter
jupyter lab
```

> ℹ️ Los notebooks esperan encontrar `book1.csv` **en la misma carpeta**. Si mueves el archivo, actualiza la variable `RUTA` en la primera celda.

---


---

## 🧪 Cómo resolver los ejercicios

1. Ejecuta la celda de **configuración** y resuelve los ejercicios **en orden**.
2. Escribe tu código donde dice `# TU CÓDIGO AQUÍ`; **no modifiques** las líneas de *Verificación*.
3. Usa **exactamente los nombres de variables** que pide cada enunciado.
4. Interpreta el resultado de la verificación:
   - ✅ Correcto
   - ❌ Revisa tu respuesta
   - ⏳ Aún sin resolver
5. Las respuestas de texto (✍️) se escriben en la celda de Markdown indicada.
6. Antes de entregar: **Kernel → Restart & Run All** y confirma que no hay errores.


## 🛠️ Requisitos

- Python **3.9 o superior**
- `pandas`, `numpy`, `matplotlib`, `seaborn`, `jupyterlab` (ver [`requirements.txt`](requirements.txt))
- *(Opcional)* `RISE` para presentar la clase

---

## 📚 Referencias

- Tukey, J. W. (1977). *Exploratory Data Analysis*. Addison-Wesley.
- McKinney, W. *Python for Data Analysis* (autor de pandas). O'Reilly.
- Documentación: [pandas](https://pandas.pydata.org/docs/) · [seaborn](https://seaborn.pydata.org/) · [matplotlib](https://matplotlib.org/)

---

## 📝 Licencia y uso

Material con fines **educativos**. 

**Autor:** Alex Mora
