# Data Modeling con Python

Colección de notebooks educativos que implementan, paso a paso, los modelos de análisis de datos más usados en ciencia de datos — para quien está aprendiendo Machine Learning y quiere ver cada algoritmo aplicado a un caso de uso realista, no solo la teoría.

<!-- COMPLETAR: agrega un GIF o captura de pantalla mostrando una de las visualizaciones generadas por los notebooks (ej. el árbol de decisión, los clusters de K-means o la curva ROC), ya que no se pudo generar una imagen sin ejecutar el código -->

## Problema / Motivación

Investigación de algoritmos de Ciencia de Datos.

## Demo

<!-- COMPLETAR: no hay demo pública ni link desplegado en el repositorio (no hay Dockerfile, CI/CD ni configuración de hosting). Si no vas a desplegar nada, reemplaza esta sección con capturas de las gráficas/resultados de cada notebook -->

## Stack técnico

- **Lenguaje**: Python (Jupyter Notebooks)
- **Machine Learning / Estadística**: `scikit-learn`, `statsmodels`, `mlxtend`
- **Manipulación de datos**: `pandas`, `numpy`
- **Visualización**: `matplotlib`, `seaborn`
- **Entorno de ejecución**: Jupyter Notebook
- **Infraestructura/Deploy**: <!-- COMPLETAR: no se encontró Dockerfile, workflow de CI/CD ni configuración de despliegue en el repositorio. Indica si este proyecto corre solo localmente o si planeas publicarlo en algún servicio (Binder, Colab, etc.) -->

## Características principales

- **Árboles de Decisión** ([1_arboles_decision.ipynb](1_arboles_decision.ipynb)): clasificación de especies de flores Iris, con visualización del árbol y análisis de importancia de características.
- **Regresión Logística** ([2_regresion_logistica.ipynb](2_regresion_logistica.ipynb)): clasificación binaria de tumores (maligno/benigno), con curva ROC, AUC y validación cruzada.
- **Regresión Lineal** ([3_regresion_lineal.ipynb](3_regresion_lineal.ipynb)): predicción de precios de vivienda, con análisis de residuos y métricas R², MSE, RMSE y MAE.
- **ARIMA** ([4_arima.ipynb](4_arima.ipynb)): forecasting de series temporales sobre pasajeros aéreos, con test de Dickey-Fuller y análisis ACF/PACF.
- **K-means** ([5_kmeans.ipynb](5_kmeans.ipynb)): segmentación de clientes mediante clustering, con método del codo y Silhouette Score.
- **Apriori** ([6_apriori.ipynb](6_apriori.ipynb)): reglas de asociación para análisis de canasta de mercado (soporte, confianza y lift).

## Cómo correrlo localmente

```bash
# 1. Clonar el repositorio
git clone https://github.com/liazamudio/tool-data-modeling-python.git
cd tool-data-modeling-python

# 2. Crear y activar un entorno virtual (opcional pero recomendado)
python -m venv venv
venv\Scripts\activate      # Windows
source venv/bin/activate   # macOS / Linux

# 3. Instalar dependencias
pip install -r requirements.txt

# 4. Iniciar Jupyter Notebook
jupyter notebook
```

No se requieren variables de entorno ni servicios externos: cada notebook genera o descarga sus propios datos de ejemplo (datasets sintéticos o estándar de `scikit-learn`) al ejecutarse.

Abre cualquiera de los `.ipynb` desde la interfaz de Jupyter y ejecuta las celdas en orden.

## Decisiones técnicas relevantes

<!-- COMPLETAR: no se puede inferir del código por qué se eligió scikit-learn/statsmodels/mlxtend sobre otras alternativas, ni qué trade-offs se consideraron (por ejemplo, notebooks vs. scripts, datasets sintéticos vs. reales). Agrega esa justificación si es relevante -->

## Estado del proyecto

<!-- Indica el estado real (Activo / Mantenido / Archivado) -->
Archivado por el momento.

## Autor / Rol

Alex Zamudio

## Licencia

[MIT](LICENSE)
