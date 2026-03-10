# Predicción de Cancelación de Clientes (Churn)

## Descripción
Este proyecto desarrolla modelos predictivos de Machine Learning para identificar clientes con mayor probabilidad de cancelar sus servicios (churn). El objetivo es ayudar a la empresa a anticiparse a la cancelación y diseñar estrategias de retención basadas en datos.

El análisis se realizó utilizando Python en Google Colab, aplicando técnicas de preprocesamiento de datos, entrenamiento de modelos y evaluación de desempeño.

---

## Objetivos
- Preparar los datos para el modelado (tratamiento, codificación y normalización).
- Analizar correlaciones y seleccionar variables relevantes.
- Entrenar modelos de clasificación.
- Evaluar el rendimiento de los modelos mediante métricas.
- Interpretar la importancia de variables.
- Identificar factores que influyen en la cancelación de clientes.

---

## Tecnologías utilizadas

- Python
- pandas
- numpy
- scikit-learn
- imblearn
- seaborn
- matplotlib

Entorno de trabajo: Google Colab

---

## Dataset

Para ejecutar el proyecto es necesario cargar el archivo:
Datos_tratados.csv

## Modelos utilizados

Se entrenaron dos modelos de clasificación:

- Árbol de decisión
- K-Nearest Neighbors (KNN)

---

## Evaluación de modelos

Se utilizaron las siguientes métricas:

- Accuracy
- Precision
- Recall
- F1-score
- Matriz de confusión

| Modelo | Accuracy | Precision | Recall | F1-score |
|------|------|------|------|------|
| Árbol de decisión | 0.69 | 0.71 | 0.65 | 0.68 |
| KNN | 0.66 | 0.65 | **0.71** | 0.68 |

El Árbol de decisión obtuvo mejor precisión y exactitud, mientras que KNN presentó mayor recall, lo que permite detectar más clientes que cancelan el servicio.

---

## Variables más relevantes

Las variables con mayor influencia en la cancelación fueron:

- **tenure** (tiempo del cliente en la empresa)
- **Contract_Month-to-month**
- **Charges.Total**
- **Charges.Monthly**
- **PaymentMethod_Electronic check**
- **OnlineSecurity**

La variable **tenure** fue el factor más importante en ambos modelos.

---

## Conclusión

Los resultados muestran que la cancelación de clientes está fuertemente relacionada con:

- menor **antigüedad del cliente**
- **contratos mensuales**
- **costos del servicio**

Estos resultados permiten identificar clientes con mayor riesgo de abandono y diseñar estrategias de retención, como incentivar contratos de mayor duración y ofrecer beneficios a clientes con baja antigüedad.


