# 🚢 Titanic Survival Analysis – EDA & Logistic Regression

## 📌 Descripción del proyecto

Este proyecto desarrolla un **Análisis Exploratorio de Datos (EDA)** completo sobre el dataset clásico del Titanic (Kaggle), con el objetivo de identificar los factores que influyeron en la supervivencia de los pasajeros y construir un modelo predictivo basado en **Regresión Logística**.

El análisis combina limpieza, transformación, ingeniería de variables y modelado estadístico con un enfoque interpretativo orientado a negocio.

---

## 🎯 Objetivos

- Comprender la estructura y calidad del dataset.
- Identificar patrones relevantes asociados a la supervivencia.
- Generar nuevas variables con valor explicativo.
- Construir un modelo de **Regresión Logística** interpretable.
- Evaluar la importancia estadística de los predictores.

---

## 🧹 Preparación y Calidad de Datos

- 891 observaciones analizadas.
- Tratamiento de valores nulos mediante:
  - Mediana (variables numéricas).
  - Moda (variables categóricas).
- Eliminación de variables no informativas: `Name`, `PassengerId`, `Ticket`.
- Ingeniería de variables:
  - `Age_group` (segmentación por grupos de edad).
  - `Is_alone` (indicador de si el pasajero viajaba solo).

---

## 📊 Principales Hallazgos del EDA

### Perfil general

- 61.6% de los pasajeros no sobrevivieron.
- 64.7% eran hombres.
- 55.1% viajaban en tercera clase.
- Edad media: 30 años.
- 72.5% embarcaron en Southampton.

### Factores asociados a la supervivencia

Se encontraron asociaciones estadísticamente significativas entre supervivencia y:

- `Sex`
- `Pclass`
- `Embarked`
- `Age_group`
- `Is_alone`

Las variables numéricas `SibSp`, `Parch` y `Fare` también mostraron diferencias relevantes entre grupos.

---

## 📈 Modelo Predictivo – Regresión Logística

La regresión logística permitió:

- Modelar la probabilidad de supervivencia.
- Identificar variables estadísticamente significativas.
- Interpretar resultados mediante *odds ratios*.

### 🔎 Variables más influyentes

- `Sex_male` → Factor de riesgo (menor probabilidad de supervivencia).
- `Pclass_3` → Factor de riesgo.
- `Age_group_Young_Adult` → Factor de riesgo.
- `Is_alone_Not_Alone` → Factor protector.

Esto confirma que el género y la clase socioeconómica fueron determinantes clave, además del contexto familiar.

---

## 💡 Valor Profesional del Proyecto

Este trabajo demuestra:

- Capacidad de limpieza y estructuración de datos reales.
- Análisis estadístico riguroso.
- Ingeniería de variables con criterio analítico.
- Modelado supervisado interpretable.
- Comunicación clara de insights accionables.

---

## 🛠️ Tecnologías utilizadas

- Python  
- Pandas  
- NumPy  
- Matplotlib / Seaborn  
- Scikit-learn  
- Statsmodels  

---

## 📌 Conclusión

El análisis confirma que la supervivencia en el Titanic no fue aleatoria: estuvo fuertemente influenciada por factores demográficos y socioeconómicos. La combinación de EDA profundo y modelado estadístico permite transformar datos históricos en insights interpretables y cuantificables.
