# 📡 Telecom X: Predicción de Cancelación de Clientes (Churn)

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Data%20Analysis-Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)



## 🎯 Objetivos del Proyecto
* **Preprocesamiento:** Limpieza, codificación de variables categóricas (One-Hot Encoding) y normalización de datos.
* **Análisis de Correlación:** Identificación de las variables con mayor impacto en la cancelación.
* **Modelado:** Entrenamiento y comparación de modelos de clasificación (Regresión Logística y Random Forest).
* **Evaluación:** Análisis de rendimiento mediante Accuracy, Precision, Recall, F1-Score y Matrices de Confusión.
* **Estrategia:** Generación de insights para la toma de decisiones de negocio.



## 🛠️ Stack Tecnológico
* **Lenguaje:** Python 3.12
* **Librerías principales:**
    * `Pandas`: Manipulación y limpieza de datos.
    * `Matplotlib` & `Seaborn`: Visualización de datos y matrices de correlación.
    * `Scikit-Learn`: Modelado predictivo, escalado y métricas de evaluación.
    * `Imbalanced-Learn`: Balanceo de clases (SMOTE).

## 📈 Hallazgos Principales (Insights)
Tras el análisis de importancia de variables, se identificaron los siguientes puntos críticos:
1.  **Tipo de Contrato:** Los contratos "Mes a mes" son el principal predictor de abandono.
2.  **Servicio de Internet:** Los usuarios de **Fibra Óptica** presentan una tasa de cancelación inusualmente alta.
3.  **Permanencia (Tenure):** Los primeros 6 a 12 meses representan el periodo de mayor riesgo de fuga.



## 🧪 Comparación de Modelos
Se evaluaron dos modelos principales para balancear la precisión global con la capacidad de detectar cancelaciones reales:

| Modelo | Exactitud (Accuracy) | Recall (Sensibilidad) | Diagnóstico |
| :--- | :---: | :---: | :--- |
| **Regresión Logística** | 74.0% | **78.6%** | **Ganador:** Alta capacidad de detección. |
| **Random Forest** | 78.6% | 48.4% | Presentó Overfitting (sobreajuste). |

## 🚀 Conclusiones y Estrategia
El modelo de **Regresión Logística** fue seleccionado como el motor predictivo principal debido a su alto **Recall**, permitiendo a Telecom X identificar a casi 8 de cada 10 clientes en riesgo. 

**Recomendaciones:**
* Migrar clientes de contrato mensual a anual mediante incentivos.
* Auditar técnicamente el servicio de Fibra Óptica.
* Implementar programas de lealtad específicos para clientes con menos de un año de antigüedad.

## ⚙️ Cómo ejecutar el proyecto
1. Clonar el repositorio.
2. Asegurarse de tener instalado `requirements.txt`.
3. Ejecutar el notebook en Google Colab o Jupyter para visualizar el pipeline completo.

---
*Proyecto desarrollado para el desafío Telecom X Alura Latam.*
