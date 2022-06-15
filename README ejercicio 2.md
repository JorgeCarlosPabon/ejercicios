# ejercicios
Jorge Carlos Pabon Sueldo

CONTEXTO DE PROBLEMA
Contexto
Según la Organización Mundial de la Salud (OMS), el accidente cerebrovascular (stroke) es la segunda causa de muerte en todo el mundo, 
responsable de aproximadamente el 11% del total de muertes. Este conjunto de datos se utiliza para predecir si es probable que un paciente sufra un 
accidente cerebrovascular en función de los parámetros de entrada como el sexo, la edad, diversas enfermedades y el tabaquismo. 
Cada fila de los datos proporciona información relevante sobre el paciente.

DATASET
Puede descargar el dataset aqui: https://neuraldojo.org/media/stroke/archive.zip

Información del dataset:
- id: identificador único
- gender: "Masculino", "Femenino" u "Otro"
- age: edad del paciente
- hypertension: 0 si el paciente no tiene hipertensión, 1 si el paciente tiene hipertensión
- heart_disease: 0 si el paciente no tiene ninguna enfermedad del corazón, 1 si el paciente tiene una enfermedad del corazón
- ever_married: "No" o "Sí"
- work_type: "niños", "Govt_jov", "Never_worked", "Private" o "Self-employment"
- Residence_type: "Rural" o "Urban"
- avg_glucose_level: nivel promedio de glucosa en sangre
- IMC: índice de masa corporal
- smoking_status: "anteriormente fumó", "nunca fumó", "fuma" o "Desconocido"*
- stroke: 1 si el paciente tuvo un stroke o 0 en caso contrario

La estructura del data set es la siguiente:

 #   Column             Non-Null Count  Dtype  
---  ------             --------------  -----  
 0   id                 5110 non-null   int64  
 1   gender             5110 non-null   object 
 2   age                5110 non-null   float64
 3   hypertension       5110 non-null   int64  
 4   heart_disease      5110 non-null   int64  
 5   ever_married       5110 non-null   object 
 6   work_type          5110 non-null   object 
 7   Residence_type     5110 non-null   object 
 8   avg_glucose_level  5110 non-null   float64
 9   bmi                4909 non-null   float64
 10  smoking_status     5110 non-null   object 
 11  stroke             5110 non-null   int64 


Se debe cambiar el tipo de dato de los objetos que deben ser numericos. 
Se debe seleccionar los los datos que no sean relevantes para el estudio de Machine Learning.

Tabajamos con 5 columnas para la fase de entrenamiento, ya que si trabajamos con mas columnas que tienen datos irrelevante se obtiene mayor procentaje de error.
hypertension
heart_disease
avg_glucose_level
smoking_status
stroke

Requerimiento y librerias:
1. importamos los archivos creados en excel con la extension .csv (from  google.colab import files)
2. importamos las librerias pandas para leer archivos (import pandas as pd)
3. importamos matplotlib para mostrar graficas(import matplotlib.pyplot as plt)
4. importamos sklearn para hacer predicciones en modelo lineal (sklearn.linear_model import LinearRegression)
5. importamos numpy para mostrar el error (import numpy as np from sklearn.metrics import mean_squared_error)
6. importamos el arbol de decision de maching learning (import tree)
7. importamos neural_network  para clasificar los datos(.neural_network import MLPClassifier)

CONCLUSION Y RESULTADOS
Algoritmo Lineal
con los valores de:
hypertension	heart_disease	avg_glucose_level	stroke
0.0		1.0			191.61		1
La probabilidad de enfermedad es de 2%

Algoritmo de arboles:
Con los mismos valores se tiene una probabilidad de 3%

Agoritmo de red neuronal:
Con los mismos valores se tiene una probabilidad de 2%

En conclusion se puede establecer que se puede entrenar el ML para poder definir la probabilidad de STROKE.
