# Análisis de Componentes Principales (PCA) — Iris

![Python](https://img.shields.io/badge/Python-3.8+-blue)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange)
![Status](https://img.shields.io/badge/Status-Académico-green)

Autor: Jorge Enrique Serangelli Andrade – 596711  
Fecha: 16 de febrero de 2026  

---

## Descripción

Este repositorio contiene la implementación completa del Análisis de Componentes Principales (PCA) aplicado al dataset Iris.

El proyecto incluye análisis exploratorio de datos, estudio de correlaciones entre variables, reducción de dimensionalidad y visualización de los componentes principales en espacios de menor dimensión.

El objetivo es comprender la estructura del dataset, identificar redundancia entre variables y evaluar qué tanta información puede conservarse al reducir dimensiones, especialmente para aplicaciones de clasificación mediante modelos neuronales.

---

## Dataset

Fuente: UCI Machine Learning Repository — Iris  
URL: https://archive.ics.uci.edu/dataset/53/iris  

El dataset contiene mediciones de flores pertenecientes a tres especies:

- Iris setosa  
- Iris versicolor  
- Iris virginica  

Cada observación incluye cuatro variables numéricas:

- Longitud del sépalo  
- Ancho del sépalo  
- Longitud del pétalo  
- Ancho del pétalo  

La variable objetivo corresponde a la especie de la flor, por lo que se trata de un problema de clasificación multiclase.

---

## Contenido del proyecto

Archivo principal:

Assignment_3_Principal_Component_Analysis.ipynb

El notebook incluye:

Exploración de datos 
- estadísticos descriptivos  
- histogramas de distribución  
- matriz de correlación entre variables  

Preparación de datos
- estandarización de variables  
- análisis de relaciones lineales  

Implementación de PCA
- cálculo de matriz de covarianza  
- obtención de eigenvalores y eigenvectores  
- ordenamiento de componentes principales  
- construcción de matriz de transformación  
- proyección al nuevo espacio reducido  

Evaluación de PCA
- varianza explicada por componente  
- varianza acumulada  

Visualización
- proyección en 2 dimensiones  
- proyección en 3 dimensiones  
- separación de clases en el espacio transformado  

---

## Principales resultados

El primer componente principal explica aproximadamente 0.7278 de la varianza total.  
El segundo componente explica aproximadamente 0.2303.  

Juntos concentran la gran mayoría de la información del dataset.

Esto confirma que es posible reducir dimensionalidad manteniendo la estructura principal de los datos.

Las visualizaciones muestran:

- separación clara de una especie  
- cercanía entre las otras dos especies  
- conservación de la estructura original en menor dimensión  

---

## Relación con modelos neuronales

El dataset Iris corresponde a un problema de clasificación supervisada.

La reducción de dimensionalidad mediante PCA permite:

- eliminar redundancia entre variables correlacionadas  
- reducir complejidad del espacio de entrada  
- concentrar la información más relevante  
- simplificar la representación de los datos  

Esto puede mejorar la estabilidad del entrenamiento y la eficiencia computacional de modelos de clasificación como redes neuronales.

---

## Requisitos

Python 3.8 o superior.

Instalar dependencias:

pip install -r requirements.txt

---

## Instrucciones para ejecutar

1. Crear entorno virtual (recomendado)

Windows:

python -m venv .venv  
.\.venv\Scripts\Activate.ps1  

Mac / Linux:

python3 -m venv .venv  
source .venv/bin/activate  

---

2. Instalar dependencias

pip install -r requirements.txt

---

3. Ejecutar notebook

jupyter notebook Assignment_3_Principal_Component_Analysis.ipynb

---

## Resultados esperados

Al ejecutar el notebook se obtendrá:

- matriz de correlación entre variables  
- histogramas de distribución  
- La varianza de los componentes  
- proyección PCA en 2D  
- proyección PCA en 3D  
- visualización de separación entre especies  

---

## Notas

El dataset se descarga automáticamente desde UCI, por lo que no es necesario descargar archivos manualmente.

El análisis puede reutilizarse para otros datasets ajustando la variable objetivo.

---

## Créditos

Notebook y análisis realizados por Jorge Enrique Serangelli Andrade  
Matrícula 596711

---

## Licencia

Uso académico y con fines de aprendizaje.  
Si reutilizas el material, cita al autor.

