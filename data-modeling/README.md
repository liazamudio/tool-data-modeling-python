# Modelos de Análisis de Datos - Data Modeling

Este directorio contiene notebooks de Python que implementan y explican diferentes modelos de análisis de datos, tanto supervisados como no supervisados.

## 📚 Estructura de Notebooks

### Modelos Supervisados

#### 1. Clasificación

##### 🌳 1_arboles_decision.ipynb - Árboles de Decisión
**Descripción**: Los árboles de decisión son modelos que toman decisiones mediante una serie de preguntas basadas en las características de los datos.

**Caso de uso**: Clasificación de especies de flores Iris basándose en características como longitud y ancho de pétalos y sépalos.

**Características principales**:
- Fácil interpretación y visualización
- No requiere normalización de datos
- Maneja variables categóricas y numéricas
- Visualización del árbol de decisión
- Análisis de importancia de características

**Librerías utilizadas**: `sklearn`, `pandas`, `matplotlib`, `seaborn`

---

##### 📊 2_regresion_logistica.ipynb - Regresión Logística
**Descripción**: Modelo estadístico para problemas de clasificación binaria que predice la probabilidad de pertenencia a una clase.

**Caso de uso**: Clasificación de tumores como malignos o benignos basándose en características del tumor.

**Características principales**:
- Proporciona probabilidades de clasificación
- Interpretación clara mediante coeficientes
- Curva ROC y AUC para evaluación
- Validación cruzada
- Normalización de características

**Librerías utilizadas**: `sklearn`, `pandas`, `matplotlib`, `seaborn`

---

#### 2. Regresión

##### 📈 3_regresion_lineal.ipynb - Regresión Lineal
**Descripción**: Modelo que predice valores continuos mediante una relación lineal entre variables independientes y dependientes.

**Caso de uso**: Predicción de precios de casas basándose en características como número de habitaciones, ubicación, edad, etc.

**Características principales**:
- Predicción de valores continuos
- Análisis de correlaciones
- Evaluación con R², MSE, RMSE, MAE
- Visualización de residuos
- Análisis de coeficientes

**Librerías utilizadas**: `sklearn`, `pandas`, `matplotlib`, `seaborn`, `numpy`

---

#### 3. Series de Tiempo

##### ⏱️ 4_arima.ipynb - ARIMA (AutoRegressive Integrated Moving Average)
**Descripción**: Modelo estadístico para análisis y predicción de series temporales que combina autoregresión, integración y media móvil.

**Caso de uso**: Predicción de número de pasajeros aéreos mensuales basándose en datos históricos.

**Características principales**:
- Descomposición de series temporales (tendencia, estacionalidad, residuo)
- Prueba de estacionariedad (Test de Dickey-Fuller)
- Análisis ACF y PACF
- Predicciones futuras
- Análisis de residuos

**Librerías utilizadas**: `statsmodels`, `pandas`, `matplotlib`, `seaborn`, `sklearn`

---

### Modelos No Supervisados

#### 1. Agrupamiento (Clustering)

##### 🎯 5_kmeans.ipynb - K-means
**Descripción**: Algoritmo de clustering que agrupa datos en k clusters basándose en similitud de características.

**Caso de uso**: Segmentación de clientes de un centro comercial en grupos basándose en edad, ingreso y comportamiento de gasto.

**Características principales**:
- Método del codo para determinar k óptimo
- Silhouette Score para evaluación
- Visualizaciones 2D y 3D de clusters
- Análisis de centroides
- Perfiles de segmentos

**Librerías utilizadas**: `sklearn`, `pandas`, `matplotlib`, `seaborn`, `mpl_toolkits`

---

#### 2. Reglas de Asociación

##### 🛒 6_apriori.ipynb - Apriori
**Descripción**: Algoritmo de minería de datos que descubre reglas de asociación entre elementos en transacciones.

**Caso de uso**: Análisis de canasta de mercado para descubrir qué productos se compran juntos frecuentemente.

**Características principales**:
- Cálculo de soporte, confianza y lift
- Identificación de patrones de compra
- Visualización de reglas
- Análisis de productos específicos
- Recomendaciones de negocio

**Librerías utilizadas**: `mlxtend`, `pandas`, `matplotlib`, `seaborn`, `numpy`

---

## 🚀 Cómo Usar los Notebooks

### Requisitos Previos

Instalar las dependencias necesarias:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn statsmodels mlxtend jupyter
```

### Ejecución

1. Navegar al directorio:
```bash
cd data-modeling
```

2. Iniciar Jupyter Notebook:
```bash
jupyter notebook
```

3. Abrir el notebook deseado y ejecutar las celdas secuencialmente.

---

## 📊 Estructura de Cada Notebook

Todos los notebooks siguen una estructura similar:

1. **Introducción y Descripción**: Explicación del modelo y caso de uso
2. **Importación de Librerías**: Configuración del entorno
3. **Carga y Exploración de Datos**: Análisis exploratorio del dataset
4. **Preparación de Datos**: Limpieza, normalización y división de datos
5. **Entrenamiento del Modelo**: Configuración y entrenamiento
6. **Predicciones**: Generación de predicciones
7. **Evaluación**: Métricas de rendimiento
8. **Visualizaciones**: Gráficos explicativos
9. **Conclusiones**: Resumen de hallazgos y aplicaciones

---

## 📖 Conceptos Clave

### Aprendizaje Supervisado
Los modelos aprenden de datos etiquetados (entrada + salida conocida) para hacer predicciones sobre nuevos datos.

### Aprendizaje No Supervisado
Los modelos encuentran patrones ocultos en datos sin etiquetas, agrupando o asociando elementos similares.

### Métricas de Evaluación

**Clasificación**:
- Accuracy (Precisión)
- Precision (Exactitud)
- Recall (Sensibilidad)
- F1-Score
- AUC-ROC

**Regresión**:
- R² (Coeficiente de determinación)
- MSE (Error Cuadrático Medio)
- RMSE (Raíz del Error Cuadrático Medio)
- MAE (Error Absoluto Medio)

**Clustering**:
- Silhouette Score
- Davies-Bouldin Index
- Inercia

**Reglas de Asociación**:
- Soporte
- Confianza
- Lift

---

## 🎓 Objetivos de Aprendizaje

Al completar estos notebooks, comprenderás:

✅ Diferencias entre aprendizaje supervisado y no supervisado
✅ Cuándo aplicar cada tipo de modelo
✅ Cómo preparar datos para machine learning
✅ Interpretación de métricas de evaluación
✅ Visualización de resultados
✅ Aplicaciones prácticas de cada modelo

---

## 🔧 Personalización

Cada notebook puede ser modificado para:
- Usar tus propios datasets
- Ajustar hiperparámetros
- Probar diferentes configuraciones
- Experimentar con otras visualizaciones

---

## 📝 Notas Importantes

- Los notebooks usan datos sintéticos generados para fines educativos
- Todos los ejemplos están completamente documentados
- Se incluyen visualizaciones para facilitar la comprensión
- Los códigos son reproducibles (semilla aleatoria fijada)

---

## 🤝 Contribuciones

Estos notebooks son recursos educativos. Siéntete libre de:
- Modificar y experimentar
- Añadir tus propios análisis
- Crear versiones extendidas
- Compartir con otros estudiantes

---

## 📚 Referencias y Recursos Adicionales

- [Scikit-learn Documentation](https://scikit-learn.org/)
- [Statsmodels Documentation](https://www.statsmodels.org/)
- [MLxtend Documentation](http://rasbt.github.io/mlxtend/)
- [Pandas Documentation](https://pandas.pydata.org/)

---

**Autor**: Generado para fines educativos
**Fecha**: Noviembre 2025
**Versión**: 1.0
