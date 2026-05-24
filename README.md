# Clasificación de Lesiones Cutáneas con Inteligencia Artificial

Proyecto enfocado en la clasificación de lesiones cutáneas benignas y malignas a partir del dataset HAM10000, explorando enfoques de aprendizaje supervisado, no supervisado y deep learning para el análisis de imágenes dermatológicas.

## Dataset utilizado

Este proyecto utiliza el dataset **HAM10000 (Human Against Machine with 10000 training images)**, un conjunto de datos dermatológico ampliamente utilizado para clasificación de lesiones cutáneas.

**Fuente:**  
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

## Carga de datos

Los notebooks cargan automáticamente los archivos CSV mediante enlaces públicos de Google Drive, por lo que no es necesario descargar manualmente el dataset completo para ejecutar los experimentos actuales.

```python
def cargar_csv(file_id):
    url = f"https://drive.google.com/uc?export=download&id={file_id}"
    return pd.read_csv(StringIO(requests.get(url).text))

meta     = cargar_csv("1HAcuf87ADCTFmT048xkx9LImkwnPjWwR")
ham8_l   = cargar_csv("1STRxSq4TZfNoS3SWKVtHzn4swVRx2wCU")
ham8_rgb = cargar_csv("1xfd7LOevJ-ueN4EufCK9tezH5tOq_sGI")
ham28_l  = cargar_csv("1BaP97p2QPDSgqwtB-FAXazXHjzGQ6yLv")
ham28_rgb= cargar_csv("1c9OPTuKl8k3xAVHMSfQV5-SvsoGGXoT6")
```

## Objetivo del proyecto

El objetivo es clasificar correctamente lesiones cutáneas como benignas o malignas mediante técnicas de inteligencia artificial, buscando apoyar la detección temprana a partir del análisis de imágenes dermatológicas y datos clínicos asociados.
