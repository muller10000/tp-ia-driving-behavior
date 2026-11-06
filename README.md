# Clasificación de Comportamiento de Conducción – Trabajo Práctico de Inteligencia Artificial

Este repositorio contiene el código fuente correspondiente al **Trabajo Práctico Final Libre de la asignatura Inteligencia Artificial**.

El objetivo del proyecto es abordar la clasificación de comportamientos de conducción a partir de datos provenientes de sensores inerciales. Para ello, se implementan y evalúan distintos enfoques de aprendizaje automático, incluyendo modelos clásicos y redes neuronales, con el propósito de comparar su desempeño en la identificación de diferentes patrones de conducción.

## Informe técnico

El desarrollo metodológico y conceptual del trabajo se encuentra documentado en el **Informe Técnico**, que incluye:

- Descripción del problema y objetivos.
- Análisis del conjunto de datos y preprocesamiento.
- Marco teórico y fundamentos de los modelos implementados.
- Diseño experimental y decisiones de implementación.
- Evaluación de resultados mediante métricas de rendimiento.
- Comparación y análisis de los enfoques utilizados.

**[Consultar Informe Técnico (PDF)](./docs/Informe_Tecnico_Muller.pdf)**

## Reproducibilidad y ejecución

A continuación, se detallan los pasos necesarios para configurar el entorno y ejecutar el proyecto.

### 1. Requisitos previos

Para ejecutar el código se necesita tener instalado:

- Python 3.10 o superior.
- Git.

### 2. Instalación y configuración del entorno

Primero, clonar el repositorio y acceder al directorio del proyecto:

```bash
git clone https://github.com/TU_USUARIO/tp-ia-driving-behavior.git
cd tp-ia-driving-behavior
```

Crear y activar un entorno virtual para aislar las dependencias del proyecto:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

En Windows, la activación del entorno se realiza mediante:

```bash
.venv\Scripts\activate
```

Finalmente, instalar las dependencias necesarias:

```bash
pip install -r requirements.txt
```

## 3. Preparación de los datasets

El proyecto utiliza dos conjuntos de datos relacionados con la clasificación del comportamiento de conducción, obtenidos de distintas fuentes.

1) Dataset 1: Driving Behavior Dataset (Kaggle)

El primer conjunto de datos se obtiene desde Kaggle:

- **Fuente:** [Driver Behavior Dataset – Kaggle](https://www.kaggle.com/datasets/shashwatwork/driving-behavior-dataset)
- **Descarga:** mediante `kagglehub` o descarga manual desde la plataforma.
- **Ubicación esperada:** `data/raw/dataset_kaggle/`

Para la descarga automática, es necesario configurar previamente las credenciales de Kaggle. El procedimiento correspondiente se encuentra documentado en el notebook de preparación inicial.

Como alternativa, se puede descargar el dataset manualmente y extraer su contenido en la carpeta indicada.

2) Dataset 2: Driver Behavior Dataset (GitHub)

El segundo conjunto de datos también corresponde a un *Driver Behavior Dataset*, pero se obtiene desde un repositorio de GitHub.

- **Fuente:** [Driver Behavior Dataset – GitHub](URL_DEL_REPOSITORIO)
- **Descarga:** mediante clonación del repositorio o descarga de sus archivos.
- **Ubicación esperada:** `data/raw/dataset_github/`

Para obtenerlo mediante Git:

git clone https://github.com/jair-jr/driverBehaviorDataset.git data/raw/dataset_github

También es posible descargar los archivos directamente desde GitHub y ubicarlos en la carpeta correspondiente.

### Consideraciones

Ambos datasets se mantienen separados dentro de `data/raw/` para preservar su procedencia y permitir su procesamiento y evaluación de manera independiente.

Los notebooks del proyecto documentan las tareas de exploración, preparación y preprocesamiento necesarias para trabajar con cada conjunto de datos.