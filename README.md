# Evaluación de datos sintéticos para la estimación de la Probabilidad de Default mediante Machine Learning y XAI

Repositorio asociado al Trabajo Fin de Máster (TFM) del Máster Universitario 
en Big Data y Ciencia de Datos de la Universidad Internacional de Valencia (VIU).

## Descripción

Este repositorio contiene los notebooks utilizados para el desarrollo experimental
del Trabajo Fin de Máster.

El estudio evalúa la utilidad de datos sintéticos para la estimación de la
Probabilidad de Default (PD) mediante modelos de Machine Learning, considerando
tres dimensiones principales:

1. Fidelidad estadística respecto a los datos reales.
2. Utilidad predictiva para la estimación de la PD.
3. Consistencia explicativa mediante técnicas de Inteligencia Artificial
   Explicable (XAI).

Como caso de estudio se utiliza el conjunto de datos Home Credit Default Risk.

## Objetivo

El objetivo general del trabajo es evaluar la utilidad de los datos sintéticos
para la estimación de la Probabilidad de Default mediante modelos de Machine
Learning, considerando su similitud respecto a los datos reales, su utilidad
predictiva y la consistencia de las explicaciones obtenidas mediante
Inteligencia Artificial Explicable (XAI).

## Metodología

El desarrollo experimental sigue como referencia la metodología CRISP-DM.

El proceso comprende las siguientes etapas:

- Comprensión de los datos.
- Preparación de los datos.
- Generación de datos sintéticos.
- Evaluación de fidelidad estadística.
- Evaluación de utilidad predictiva.
- Modelado final de la Probabilidad de Default.
- Evaluación de consistencia explicativa mediante SHAP.
- Evaluación integrada de los resultados.

## Estructura del repositorio

Los notebooks se encuentran organizados siguiendo el flujo experimental del TFM.

### 01_Data_Understanding_02_Data_Preparation

Comprensión y preparación del conjunto de datos original.

Incluye el análisis exploratorio, evaluación de calidad, tratamiento de valores
faltantes, transformación de variables e ingeniería de características.

Corresponde principalmente a las fases Data Understanding y Data Preparation
de CRISP-DM.

### 03_Synthetic_Data

Primera fase de generación y evaluación de datos sintéticos mediante diferentes
métodos para datos tabulares.

### 04_Modelling

Primera evaluación experimental de la utilidad predictiva de los datos
sintéticos mediante modelos de Machine Learning.

### 05_Synthetic_Data_Optimization

Optimización del proceso de generación de datos sintéticos a partir de los
resultados obtenidos en los experimentos iniciales.

### 06_Synthetic_Model_Comparison

Comparación de los conjuntos de datos sintéticos mediante métricas de fidelidad
estadística y utilidad predictiva.

Esta etapa permite seleccionar el conjunto sintético utilizado posteriormente
en la comparación final.

### 07_Final_PD_Modeling

Entrenamiento y evaluación final de modelos para la estimación de la
Probabilidad de Default.

Se comparan modelos entrenados con datos reales y datos sintéticos bajo
condiciones experimentales equivalentes.

### 08_XAI

Evaluación de la consistencia explicativa entre los modelos entrenados con
datos reales y sintéticos mediante SHAP.

Se analizan explicaciones tanto a nivel global como a nivel de observaciones
individuales.

### 09_Evaluacion_integrada_y_conclusiones_finales

Integración de los resultados obtenidos en las tres dimensiones evaluadas:

- Fidelidad estadística.
- Utilidad predictiva.
- Consistencia explicativa.

## Orden de ejecución

Para reproducir el flujo experimental completo, los notebooks deben ejecutarse
en el siguiente orden:

01 → 03 → 04 → 05 → 06 → 07 → 08 → 09

Las fases 01 y 02 de comprensión y preparación de los datos se encuentran
integradas en el primer bloque del proyecto.

## Datos

El conjunto de datos utilizado como punto de partida corresponde a
Home Credit Default Risk.

Los datasets originales y determinados archivos intermedios generados durante
los experimentos no se almacenan directamente en este repositorio.

Los notebooks documentan los procedimientos utilizados para la preparación
de los datos y la generación de los conjuntos sintéticos empleados durante
la investigación.

## Modelos evaluados

Durante el estudio se consideran diferentes algoritmos de Machine Learning
para la estimación de la Probabilidad de Default, entre ellos:

- Regresión Logística
- Random Forest
- XGBoost
- LightGBM

## Generación de datos sintéticos

Se evalúan diferentes métodos de generación de datos sintéticos tabulares,
incluyendo:

- Gaussian Copula
- CTGAN
- TVAE

La selección del conjunto sintético final se realiza considerando conjuntamente
su fidelidad estadística y su utilidad predictiva.

## Evaluación

La evaluación experimental considera tres dimensiones complementarias:

### Fidelidad estadística

Se analiza el grado en que los datos sintéticos reproducen propiedades y
relaciones presentes en los datos reales.

### Utilidad predictiva

Se evalúa la capacidad de los datos sintéticos para entrenar modelos capaces
de generalizar sobre datos reales mediante escenarios experimentales
comparables.

### Consistencia explicativa

Se utiliza SHAP para analizar las similitudes y diferencias entre las
explicaciones generadas por modelos entrenados con datos reales y sintéticos.

## Requisitos

El proyecto ha sido desarrollado principalmente en Python mediante notebooks.

Las principales librerías utilizadas se encuentran especificadas en el archivo:

requirements.txt

## Reproducibilidad

Los notebooks han sido organizados siguiendo el orden del proceso experimental
descrito en la memoria del TFM.

Algunos archivos de datos intermedios no se incluyen debido a su tamaño. Estos
archivos se generan durante las distintas etapas del pipeline experimental.

## Entorno de ejecución y dependencias

El desarrollo experimental se realizó en Google Colab, utilizando Python y las librerías necesarias para el procesamiento de datos, la generación de datos sintéticos, el entrenamiento de modelos de Machine Learning y el análisis de explicabilidad mediante SHAP.

Las principales dependencias del proyecto se encuentran documentadas en el archivo requirements.txt.

Para instalar las dependencias en un entorno compatible, se puede ejecutar el siguiente comando:

pip install -r requirements.txt

La ejecución de los notebooks requiere disponer de los conjuntos de datos correspondientes y configurar las rutas de acceso a los archivos.

## Autor

Jorge Durán

Trabajo Fin de Máster  
Máster Universitario en Big Data y Ciencia de Datos  
Universidad Internacional de Valencia (VIU)

## Version
Version 0.1.0 - Se inicializa el repositorio con arquetipo actualizado al 04/10/2026
