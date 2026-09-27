# MnistNeuralNetwork

Este repositorio contiene la resolución del Trabajo Práctico N° 1 de Aprendizaje Profundo para la Licenciatura en Ciencia de Datos de la Universidad del Gran Rosario. El objetivo principal es desarrollar y entrenar una Red Neuronal Convolucional (CNN) utilizando el dataset MNIST y evaluar su rendimiento con imágenes de dígitos manuscritos creadas de forma propia.

## Estructura del Proyecto

*   `Trabajo_Práctico_Nro_1_Aprendizaje_Profundo_BrunoPace.ipynb`: Notebook de Jupyter que contiene el código paso a paso para la carga de datos, preprocesamiento, construcción del modelo, evaluación y predicción con imágenes propias.
*   `data/`: Carpeta que contiene las imágenes de dígitos manuscritos (3 a 5 imágenes) creadas para probar el modelo.
*   `README.md`: Este archivo, con instrucciones e información del proyecto.
*   `requirements.txt`: Lista de dependencias necesarias para ejecutar el proyecto.

## Requisitos

Para ejecutar el código, se recomienda utilizar un entorno virtual de Python. Puedes crearlo utilizando `venv` o `conda`.

### 1. Clonar el repositorio

```bash
git clone https://github.com/bpace1/MnistNeuralNetwork.git
cd MnistNeuralNetwork
```

### 2. Crear un entorno virtual de Python

**Usando venv (Python estándar):**

```bash
python3 -m venv venv
source venv/bin/activate  # En Linux/macOS
venv\Scripts\activate     # En Windows
```

**Usando conda:**

```bash
conda create --name mnist_env python=3.10
conda activate mnist_env
```

### 3. Instalar dependencias

Con el entorno virtual activado, instala las librerías necesarias utilizando el archivo `requirements.txt`:

```bash
pip install -r requirements.txt
```

## Ejecución del Notebook

Puedes ejecutar el notebook en tu máquina local o en Google Colab.

### En Local (VS Code / IDE)

1. Abre la carpeta del proyecto en tu IDE (por ejemplo, **VS Code**):
   ```bash
   code .
   ```

2. Abre el archivo `Trabajo_Práctico_Nro_1_Aprendizaje_Profundo_BrunoPace.ipynb`.
3. Asegúrate de contar con la extensión de **Jupyter** instalada en tu editor.
4. Selecciona el kernel/entorno virtual de Python configurado anteriormente (`venv` o `mnist_env`) en la esquina superior derecha del notebook.
5. Ejecuta las celdas de forma interactiva y secuencial.

### En Google Colab

1. Ingresa a [Google Colab](https://colab.research.google.com/).
2. Selecciona la pestaña **Subir** (Upload) y carga el archivo `Trabajo_Práctico_Nro_1_Aprendizaje_Profundo_BrunoPace.ipynb`.
3. Ejecuta las celdas secuencialmente. El notebook está configurado para clonar automáticamente este repositorio y obtener la carpeta `data/` si no se encuentra en el entorno local.

## Resultados

El modelo implementado alcanzó un **Accuracy** y un **F1-Score** superior a **0.98**, demostrando una excelente capacidad de clasificación y un rendimiento equilibrado en todos los dígitos. La matriz de confusión confirmó la precisión del clasificador, con mínimas confusiones en dígitos morfológicamente similares.