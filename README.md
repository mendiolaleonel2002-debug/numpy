# 🧪 NumPy & Procesamiento de Imágenes en Python

Un espacio dedicado al aprendizaje práctico de **NumPy**, **Ciencia de Datos**, manipulación de arreglos multidimensionales y análisis de imágenes utilizando Python y Jupyter Notebooks.

Este repositorio contiene libretas interactivas diseñadas para explorar desde los fundamentos de arreglos y estadística descriptiva hasta el procesamiento básico de imágenes digitales.

---

## 📁 Estructura del Proyecto

```text
numpy/
├── prueba.ipynb             # Introducción a Ciencia de Datos con NumPy (arrays, estadística y ventas)
├── 1_numpy_avanzado.ipynb   # NumPy avanzado: atributos de arreglos y matrices aleatorias
├── 2_ejercicios.ipynb       # Análisis completo de imagen (beagle.jpg) con Matplotlib y Pandas
├── beagle.jpg               # Imagen de muestra para el análisis visual
└── README.md                # Documentación del proyecto
```

---

## 📓 Descripción de los Notebooks

### 1. 🧑‍💻 `prueba.ipynb` - Introducción a Ciencia de Datos con NumPy
Libreta introductoria enfocada en los fundamentos de NumPy aplicados a operaciones numéricas y análisis básico de datos.

* **Conceptos y ejercicios:**
  * **Creación de arreglos y matrices:** arreglos 1D y matrices 2D ($3 \times 3$) con `np.array()`.
  * **Operaciones matemáticas vectorizadas:** suma, resta, multiplicación y división sobre arreglos completos.
  * **Funciones estadísticas:** cálculo de promedio (`np.mean()`), máximo (`np.max()`), mínimo (`np.min()`), desviación estándar (`np.std()`), mediana (`np.median()`) y suma (`np.sum()`).
  * **Análisis de ventas:** filtrado booleano de valores (`ventas >= 1000`), cálculo de ventas totales, promedio semanal, venta más alta y suma de ventas de mayor valor.

### 2. 🧮 `1_numpy_avanzado.ipynb` - NumPy Avanzado
Notebook que combina la inspección de arreglos multidimensionales de NumPy con la generación y visualización de matrices aleatorias usando Python puro.

* **Parte 1 — Arreglos NumPy:**
  * Creación de arreglos multidimensionales con `np.array()` y `dtype='float'`.
  * Inspección de atributos esenciales:
    * `.ndim`: número de dimensiones.
    * `.shape`: dimensiones en formato de tupla `(filas, columnas)`.
    * `.size`: total de elementos.

* **Parte 2 — Matrices Aleatorias:**
  * Generación dinámica de matrices cuadradas $N \times N$ con `random.randint`.
  * Formateo simétrico en consola usando f-strings y `.join()`.
  * Ejemplos con matrices de $5 \times 5$, $10 \times 10$ y $20 \times 20$.

### 3. 🖼️ `2_ejercicios.ipynb` - Análisis de una Imagen
Procesamiento digital de imágenes: cómo una fotografía se representa como una matriz tridimensional en memoria y cómo analizar sus canales de color.

* **Conceptos y análisis incluidos:**
  * Lectura y visualización de `beagle.jpg` con `plt.imread()` y `plt.imshow()`.
  * Análisis de dimensiones `(Alto, Ancho, Canales RGB)` mediante `.shape` e inspección de píxeles individuales (`img[10, 10]`) y sus componentes Rojo, Verde y Azul.
  * Estadísticas globales de intensidad: mínimo (`.min()`), máximo (`.max()`), media (`.mean()`) y desviación estándar (`.std()`).
  * Visualización independiente de los canales **Rojo**, **Verde** y **Azul** con mapas de color (`Reds`, `Greens`, `Blues`) y `plt.colorbar()`.
  * Cálculo de la intensidad promedio por canal y gráfica de barras comparativa (`plt.bar()`).
  * Conversión de la matriz 3D a formato tabular mediante `img.reshape(-1, 3)` y creación de un `DataFrame` con **Pandas** (`Rojo`, `Verde`, `Azul`).
  * Histograma de distribución de frecuencias del canal azul (`plt.hist()`).

---

## 🛠️ Requisitos e Instalación

### Dependencias Principales
* **NumPy** (`numpy`): cálculo numérico y arreglos multidimensionales.
* **Pandas** (`pandas`): manejo de datos tabulares (`DataFrame`).
* **Matplotlib** (`matplotlib`): lectura, análisis visual y graficación de imágenes y datos.
* **Jupyter** (`notebook` / `jupyterlab`): ejecución de libretas interactivas.

### Configuración del Entorno

1. **Acceder al directorio:**
   ```bash
   cd numpy
   ```

2. **Crear y activar un entorno virtual (`.venv`):**
   ```bash
   python3 -m venv .venv

   # macOS/Linux
   source .venv/bin/activate

   # Windows
   .venv\Scripts\activate
   ```

3. **Instalar dependencias:**
   ```bash
   pip install numpy pandas matplotlib notebook
   ```

4. **Iniciar Jupyter:**
   ```bash
   jupyter notebook
   ```

---

## 🚀 ¿Cómo empezar?

1. Comienza con **`prueba.ipynb`** si quieres repasar arreglos básicos, operaciones vectorizadas, estadística y filtrado de datos.
2. Continúa con **`1_numpy_avanzado.ipynb`** para explorar las propiedades de los arreglos NumPy y practicar la generación de matrices aleatorias.
3. Finaliza con **`2_ejercicios.ipynb`** para cargar `beagle.jpg` y analizar una imagen real a través de sus canales RGB, estadísticas, DataFrames e histogramas.

---
> [!NOTE]
> Este proyecto forma parte de una ruta de aprendizaje orientada a **Ciencia de Datos**, **Computación Científica** y **Procesamiento de Imágenes**. ¡Perfecto para entusiastas del análisis de datos que inician su viaje en Python!
