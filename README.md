


# Predicción de Supervivencia en el Titanic – Proyecto Final Integrador

Este repositorio contiene el código y los recursos para el Proyecto Final Integrador del Diplomado en Ciencia de Datos y Análisis Avanzado. El objetivo es predecir la supervivencia de los pasajeros del RMS Titanic utilizando técnicas de Machine Learning, siguiendo la metodología CRISP‑DM.

## Contenido

- `titanic_ml_project.ipynb`: Notebook Jupyter con todo el análisis: carga de datos, ingeniería de variables, modelado (Regresión Logística y Random Forest), evaluación de métricas y explicación de variables mediante valores SHAP.
- `data/`: Carpeta donde deben colocarse los archivos `train.csv` y `test.csv` descargados de Kaggle (ver instrucciones más abajo).
- `README.md`: Este archivo, que describe el proyecto, requisitos y cómo ejecutar el notebook.

## Requisitos

- Python 3.11 o superior.
- Librerías de Python: `pandas`, `numpy`, `scikit‑learn`, `matplotlib`. Opcionalmente, `shap` y `xgboost` si se desea experimentar con métodos adicionales de interpretabilidad o modelos más avanzados.

## Instalación

1. Clona o descarga este repositorio.
2. Crea un entorno virtual (opcional pero recomendado):

   ```bash
   python -m venv env
   source env/bin/activate


3. Instala las dependencias necesarias:

   ```bash
   pip install pandas numpy scikit-learn matplotlib
   # Si deseas usar la librería SHAP y XGBoost:
   pip install shap xgboost
   ```

## Descarga de Datos

Debes descargar los archivos `train.csv` y `test.csv` del conjunto **Titanic: Machine Learning from Disaster** de Kaggle y colocarlos en la carpeta `data/` del repositorio. Para ello:

1. Crea una cuenta en Kaggle y accede a [https://www.kaggle.com/c/titanic/data](https://www.kaggle.com/c/titanic/data).
2. Acepta los términos de la competencia y descarga los archivos `train.csv` y `test.csv`.
3. Copia ambos archivos a la ruta `data/` en tu copia local del repositorio.

## Ejecución del Notebook

1. Abre el notebook `titanic_ml_project.ipynb` con Jupyter Notebook o JupyterLab:

   ```bash
   jupyter notebook titanic_ml_project.ipynb
   ```

2. Ejecuta las celdas en orden. El notebook realiza los siguientes pasos:

   * Importación de librerías y configuración.
   * Carga del dataset.
   * Ingeniería de variables y limpieza de datos.
   * Definición de modelos (Regresión Logística y Random Forest), entrenamiento con validación cruzada y evaluación de métricas.
   * Comparación de modelos y selección del modelo final.
   * Cálculo de valores SHAP aproximados para interpretar la Regresión Logística.
   * Visualización de la importancia de las variables y explicación de los valores SHAP.

3. Al finalizar, podrás observar las métricas de cada modelo y los gráficos de valores SHAP que identifican las variables más influyentes.

## Notas sobre SHAP

El notebook incluye una aproximación manual de los valores SHAP para la Regresión Logística. Si la librería `shap` está instalada, puedes modificar el código para utilizar la implementación oficial y obtener valores más precisos. Los valores SHAP ayudan a entender cómo cada característica contribuye a aumentar o disminuir la probabilidad de supervivencia.

## Citaciones

* Datos: **Kaggle – Titanic: Machine Learning from Disaster**.
* Documentación de SHAP: [https://shap.readthedocs.io/](https://shap.readthedocs.io/).


