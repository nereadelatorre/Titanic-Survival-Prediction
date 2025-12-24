# Predicción de Supervivencia en el Titanic - Análisis y Clasificación

Este proyecto consiste en un análisis exhaustivo y la implementación de múltiples modelos de Machine Learning para predecir la supervivencia de los pasajeros del Titanic. Fue desarrollado como parte de la asignatura de **Aprendizaje Computacional**.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit__Learn-yellow)

## Descripción
El objetivo principal es aplicar técnicas de **Análisis Exploratorio de Datos (EDA)**, **Preprocesamiento** y **Modelado Predictivo** para clasificar si un pasajero sobrevivió o no, basándose en características como la edad, el sexo, la clase social y el precio del billete.

El proyecto abarca desde la limpieza de datos (imputación de nulos) hasta la comparación de métricas de rendimiento (F1-Score, Accuracy) entre diferentes algoritmos.

## Librerias utilizadas
* **Lenguaje:** Python
* **Librerías de Análisis:** Pandas, NumPy
* **Visualización:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-learn (Sklearn)

## Metodología
El flujo de trabajo seguido en el notebook (`APC_Practica_1_2024.ipynb`) incluye:

1.  **EDA (Exploratory Data Analysis):**
    * Análisis de correlaciones (mapas de calor).
    * Visualización de distribución de supervivientes por género y clase.
    * Detección de valores nulos (Age, Cabin, Embarked).

2.  **Preprocesamiento:**
    * **Imputación:** Uso de `KNNImputer` y promedios condicionados para rellenar valores faltantes en 'Age' y 'Embarked'.
    * **Ingeniería de Atributos:** Creación de la variable `HasFamily` para determinar si el pasajero viajaba solo.
    * **Codificación:** Label Encoding para variables binarias y One-Hot Encoding para categóricas.
    * **Escalado:** Estandarización de variables numéricas ('Age', 'Fare') usando `StandardScaler`.

3.  **Modelado:**
    Se entrenaron y compararon los siguientes modelos:
    * Regresión Logística
    * Árboles de Decisión (Decision Tree)
    * Random Forest
    * K-Nearest Neighbors (KNN)
    * Support Vector Machines (SVM)
    * Gradient Boosting

## 📊 Resultados Destacados
* **Factor Clave:** El género y la clase social fueron determinantes; las mujeres de primera clase tuvieron la tasa de supervivencia más alta.
* **Mejor Modelo:** El modelo **Gradient Boosting** y **Random Forest** mostraron un rendimiento superior en términos de F1-Score en comparación con modelos más simples como KNN.
* **Ingeniería de características:** La variable derivada `HasFamily` mostró una correlación positiva con la supervivencia.

## Instalación y Uso
1.  Clona el repositorio:
    ```bash
    git clone [https://github.com/tu-usuario/Titanic-Survival-Prediction.git](https://github.com/tu-usuario/Titanic-Survival-Prediction.git)
    ```
2.  Instala las dependencias:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
3.  Ejecuta el notebook:
    ```bash
    jupyter notebook APC_Practica_1_2024.ipynb
    ```

## Autores
Trabajo realizado por:
* Nerea de la Torre Veguillas
* Mara Montero Jurado
* Júlia Morán Fluvià
* Adrián Prego Gallart

Matemática Computacional y Análisis de datos, UAB
