# Eficiencia Energética en Edificios

Proyecto de Ciencia de Datos para clasificar la eficiencia energética de edificios residenciales usando 
sus características arquitectónicas y físicas, basado en el Energy Efficiency Dataset (UCI).

---

## 📌 Contexto y problemática

En el Perú, aproximadamente el **35% del consumo energético** proviene del sector residencial. Sin embargo, actualmente no existen sistemas estandarizados de clasificación energética (A–G) que permitan evaluar el desempeño energético de los edificios antes de su construcción.

La ausencia de estas herramientas limita:
- El diseño de políticas públicas de construcción sostenible.
- La certificación energética de edificaciones.
- La toma de decisiones técnicas basadas en datos.

Este proyecto propone un **enfoque analítico y predictivo** como base técnica para futuras normativas de eficiencia energética.

---

## 🎯 Objetivo del proyecto

Desarrollar un **modelo predictivo** que estime la **carga de calefacción y enfriamiento** de edificios residenciales a partir de sus características arquitectónicas, y que sirva como base para una futura **clasificación energética nacional**.

---

## 📊 Dataset

- **Fuente**: UCI Machine Learning Repository  
- **Registros**: 768 edificaciones simuladas  
- **Variables de entrada**:
  - Compacidad relativa  
  - Área de pared  
  - Área de techo  
  - Altura general  
  - Área de ventanas  
  - Distribución de ventanas  
- **Variables objetivo**:
  - Carga de calefacción
  - Carga de enfriamiento

---

## 🧠 Metodología

Se aplicó la metodología **CRISP–DM**, siguiendo las etapas:

1. Entendimiento del negocio  
2. Entendimiento de los datos (EDA completo)  
3. Preparación de datos (colinealidad, VIF, binarización de variables)  
4. Modelado predictivo  
5. Evaluación y validación  
6. Interpretación de resultados

---

## 🤖 Modelos de Machine Learning evaluados

- Regresión Lineal
- Ridge y Lasso
- Árboles de Decisión
- Random Forest
- Gradient Boosting
- AdaBoost
- K-Nearest Neighbors (KNN)
- Support Vector Regression (SVR)

La validación se realizó mediante **Leave-One-Out Cross Validation (LOO)** y conjunto de prueba.

---

## 📈 Resultados principales

- **Calefacción**:
  - Mejor desempeño: **Decision Tree / Random Forest**
  - Ajuste R² ≈ **0.99**
- **Enfriamiento**:
  - Mejor desempeño: **Gradient Boosting / Random Forest**
  - Ajuste R² ≈ **0.96**

Las variables con mayor impacto fueron:
- **Área de techo**
- **Compacidad relativa**
- **Altura general**

---

## ▶️ Ejecutar el proyecto en Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
(https://colab.research.google.com/github/di-yeferson/energy-efficiency-prediction/blob/main/Prediccion_Eficiencia_v4.ipynb)

---

## 🛠️ Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels

---

## 👤 Autor

**Quispe Huamani, Diego Yeferson**  
Estudiante de Big Data y Ciencia de Datos  
Proyecto personal de análisis predictivo aplicado al sector vivienda
