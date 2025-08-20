# TelecomX-Parte2
 #Análisis de Cancelación de Clientes (Churn) — Telecom X

#Este proyecto es parte de un desafío de ciencia de datos enfocado en analizar y predecir la cancelación de clientes (churn) en una empresa de telecomunicaciones.
El objetivo es entender qué factores influyen en la cancelación y preparar los datos para modelos de machine learning.
 Objetivo del Proyecto

El principal objetivo es identificar patrones de comportamiento en los clientes que cancelan su servicio y preparar un conjunto de datos listo para entrenar modelos predictivos.
Para ello, se aplicaron varias etapas de preprocesamiento, análisis exploratorio y selección de variables.

 Estructura del Proyecto

El proyecto está organizado en pasos claros y bien definidos:

1Preparación y Limpieza de Datos

Cargamos el archivo df_limpo.csv, previamente depurado.

Eliminamos columnas irrelevantes, como identificadores únicos (customerID).

Corregimos datos inconsistentes y estandarizamos formatos.

2 Codificación de Variables Categóricas

Se aplicó One-Hot Encoding para convertir variables categóricas en variables numéricas.

Esto nos permitió calcular correlaciones y preparar el dataset para modelos de machine learning.

3 Balanceo de Clases

Identificamos un desbalance entre clientes que cancelan y los que permanecen activos.

Implementamos SMOTE para aumentar la representación de la clase minoritaria y evitar sesgos en los modelos.

4 Normalización y Estandarización

Normalizamos las variables numéricas para que tengan la misma escala.

Esto es especialmente útil para algoritmos basados en distancia como KNN, SVM y Redes Neuronales.

5 Análisis de Correlación

Calculamos la matriz de correlación para identificar relaciones entre variables.

Creamos un heatmap interactivo y limpio para visualizar correlaciones más altas.

Seleccionamos las variables más relevantes según un umbral de correlación ≥ 0.07.

6 Top 10 Variables más Relevantes

Identificamos las 10 variables con mayor correlación con la cancelación.

Visualizamos los resultados con un gráfico de barras con etiquetas numéricas para facilitar la interpretación.

 Gráficos y Visualizaciones

El proyecto utiliza matplotlib y seaborn para crear gráficos claros y atractivos:

Heatmap filtrado → para entender la relación entre variables.

Top 10 variables correlacionadas → ranking visual de factores que más influyen en la cancelación.

Distribuciones comparativas (opcional) → para analizar el comportamiento de clientes según cada variable.

 Tecnologías Utilizadas

Python 3.10+

Google Colab → entorno principal de desarrollo.

Pandas → manipulación de datos.

NumPy → operaciones numéricas.

Seaborn / Matplotlib → visualización de datos.

Scikit-learn → preprocesamiento, balanceo y preparación de modelos.
