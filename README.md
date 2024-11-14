# papd-proyecto-final

## Autores

- Diego Morales
- Jerry Rivera
- Polo Figueroa

---

# Predicción del Producto Interno Bruto (PIB) de Guatemala

**Proyecto Final de la Maestría en Data Science en la Universidad Galileo**  
Este proyecto se realizó en el contexto de nuestro programa de posgrado en Análisis y Predicción de Datos y tiene como objetivo explorar y comparar la capacidad predictiva de métodos tradicionales de econometría y modelos avanzados de machine learning en la predicción del Producto Interno Bruto (PIB) de Guatemala, un país de economía emergente.

## Metodología

La metodología del proyecto se centra en un enfoque cuantitativo comparativo, donde comparamos la eficacia de los modelos de machine learning con métodos tradicionales de econometría. Se utilizan dos enfoques principales para la predicción del PIB:

1. **Métodos Tradicionales de Econometría:**
   - Modelos de regresión lineal y modelos autorregresivos (AR, ARIMA, SARIMA) para captar patrones históricos en las series temporales.

2. **Modelos de Machine Learning:**
   - Algoritmos como K-Nearest Neighbors, Random Forest, XGBoost, Redes Neuronales Artificiales (ANN) y Redes Neuronales Recurrentes (RNN) implementados en Python usando bibliotecas como scikit-learn y TensorFlow/Keras.

Los modelos fueron evaluados utilizando métricas de error cuadrático medio (MSE) y optimizados mediante técnicas como Grid Search y Optuna para la selección de hiperparámetros.

## Datos

- **Fuente de Datos**: Los datos macroeconómicos históricos fueron descargados de [BANGUAT](https://app1.banguat.gob.gt/ords/f?p=215:1:13889732639804:::::) (Banco de Guatemala), en el módulo de Información Estadística Económica-Financiera.
- **Período de Tiempo**: Datos trimestrales desde 2009 hasta junio de 2024.
- **Variables**: Incluyen factores económicos clave como el consumo de hogares, inversión, gasto público y exportaciones, entre otros.

## Procesamiento de Datos

1. **Preparación de Datos**: Creación de variables con rezago para predicciones basadas en períodos anteriores (por ejemplo, t-1, t-2, t-3).
2. **División del Conjunto de Datos**: Se usó el 80% de los datos para entrenamiento y el 20% para pruebas.
3. **Normalización**: Los datos fueron normalizados en el caso de redes neuronales.

## Modelado y Evaluación

Se entrenaron y evaluaron modelos econométricos y de machine learning utilizando el conjunto de datos de prueba y comparando los resultados de predicción con los datos reales de PIB. Los modelos fueron ajustados para optimizar su rendimiento en función de su MSE y se implementaron técnicas de Early Stopping y validación cruzada para evitar el sobreajuste.

## Resultados

Este proyecto permite observar si los modelos de machine learning ofrecen mayor precisión en la predicción del PIB en comparación con los métodos tradicionales, proporcionando así insights sobre la aplicabilidad de técnicas avanzadas en el análisis económico de un país en desarrollo.

## Limitaciones

La precisión de los modelos puede estar limitada por factores exógenos, como crisis económicas o eventos políticos imprevistos, además de la disponibilidad y calidad de los datos.


