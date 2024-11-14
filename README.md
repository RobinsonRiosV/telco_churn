# Telco Customer Churn Prediction

## Descripción del Proyecto
Este proyecto utiliza el conjunto de datos de Telco Customer Churn de Kaggle para predecir si un cliente abandonará la empresa (churn) o no.
El modelo de churn ayuda a identificar los factores clave que influyen en la decisión de los clientes de dejar el servicio, lo que permite a las empresas 
implementar estrategias efectivas de retención de clientes.

## Conjunto de Datos
El conjunto de datos proviene de Kaggle e incluye diversas características sobre los clientes, como:
- Información demográfica (género, edad, dependientes)
- Información sobre los servicios contratados (tipo de contrato, internet, teléfono)
- Información sobre la cuenta (forma de pago, cargo mensual, duración del contrato)
Cada fila representa a un cliente y la columna Churn indica si el cliente ha abandonado el servicio o no.

## Objetivo del Proyecto
El objetivo es construir un modelo de clasificación que prediga si un cliente se dará de baja o no en función de los datos proporcionados. 
Esto se logra a través de técnicas de preprocesamiento, ingeniería de características y modelado de datos.

## Análisis Exploratorio de Datos (EDA)
El EDA incluye:
1. Análisis de las características principales que contribuyen al churn.
2. Visualización de la distribución de variables categóricas y numéricas.
3. Identificación y tratamiento de valores nulos o faltantes.
4. Análisis de correlaciones para entender relaciones entre variables.

## Preprocesamiento de Datos
1. Limpieza de Datos: Eliminación de valores nulos y duplicados.
2. Codificación: Transformación de variables categóricas en variables numéricas.
3. Normalización/Estandarización: Escalado de variables numéricas para mejorar el rendimiento del modelo.
4. División de Datos: División en conjuntos de entrenamiento y prueba.

## Modelos Utilizados
Se probaron varios modelos de clasificación para encontrar el que mejor predice el churn, incluyendo:

. Regresión Logística
. Linear Discrimination Analysis
. Decission Tree Classifier
. Random Forest
. GaussianNB
. XGBClassifier
. LGBMClassifier

El modelo final fue seleccionado en función de su precisión, área bajo la curva (AUC) y capacidad de generalización y en este caso fue la ocmbinación de varios modelos usando Stacking Classifier.

## Resultados
El modelo final logró un accuracy del 81%, un recall de 58% y una AUC de 84% en el conjunto de prueba, lo que indica una buena capacidad de predicción en la detección de clientes propensos a churn.
