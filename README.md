# Clasificación de Lesiones Cutáneas con Inteligencia Artificial

Proyecto enfocado en la clasificación de lesiones cutáneas benignas y malignas a partir del dataset HAM10000, explorando enfoques de aprendizaje supervisado, no supervisado y deep learning para el análisis de imágenes dermatológicas.

## Dataset utilizado

Este proyecto utiliza el dataset **HAM10000 (Human Against Machine with 10000 training images)**, un conjunto de datos dermatológico ampliamente utilizado para clasificación de lesiones cutáneas.

**Fuente oficial:**  
https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000

**Descripción breve:**
- 10,015 imágenes dermatoscópicas de lesiones cutáneas.
- Información clínica asociada (edad, sexo, localización, diagnóstico).
- Imágenes originales en formato JPG.
- Versiones tabulares en CSV con representación numérica de píxeles.

**Archivos utilizados en este proyecto:**
- `HAM10000_metadata.csv`
- `hmnist_8_8_L.csv`
- `hmnist_8_8_RGB.csv`
- `hmnist_28_28_L.csv`
- `hmnist_28_28_RGB.csv`

## Obtención de los datos

Los archivos no se incluyen directamente en este repositorio debido a su tamaño.

Para reproducir los experimentos:

1. Descargar el dataset desde Kaggle:  
   https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000

2. Extraer los archivos CSV necesarios.

3. Colocarlos en una carpeta local, por ejemplo:

```bash
data/
```

de forma que la estructura quede:

```bash
data/
├── HAM10000_metadata.csv
├── hmnist_8_8_L.csv
├── hmnist_8_8_RGB.csv
├── hmnist_28_28_L.csv
└── hmnist_28_28_RGB.csv
```

4. Actualizar la ruta de carga en los notebooks según la ubicación local de los archivos.

## Objetivo del proyecto

El objetivo es clasificar correctamente lesiones cutáneas como benignas o malignas mediante técnicas de inteligencia artificial, buscando apoyar la detección temprana a partir del análisis de imágenes dermatológicas y datos clínicos asociados.
