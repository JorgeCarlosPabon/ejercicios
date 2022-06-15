# ejercicios
Jorge Carlos Pabon Sueldo

CONTEXTO DE PROBLEMA

Con el aumento en la variedad de automóviles con capacidades y características diferenciadas, como modelo, año de producción, categoría, marca, 
tipo de combustible, volumen del motor, millaje, cilindros, color, bolsas de aire y muchos más, presentamos un desafío de predicción de precios de automóviles 
para todos. Todos aspiramos a tener un automóvil dentro del presupuesto con las mejores características disponibles. 
Para resolver el problema del precio, hemos creado un conjunto de datos de 19237 para el conjunto de datos de entrenamiento y 8245 para el conjunto de datos de prueba.


DATASET
Puede descargar el dataset aqui: https://neuraldojo.org/media/carprice/archive.zip
Descripción de datos Train.csv: 19237 filas x 18 columnas (incluye columnas de precio como destino)

- IDENTIFICACIÓN
- Precio: precio de la atención (columna de destino)
- Exacción
- Fabricante
- Modelo
- Año
- Categoría
- Interior de cuero
- Tipo de combustible
- Volumen del motor
- Kilometraje
- Cilindros
- Tipo de caja de cambios
- Ruedas motrices
- puertas
- Rueda
- Color
- bolsas de aire

Se debe cambiar el tipo de dato de los objetos que deben ser numericos. 

Seleccionamos los datos que no sean relevantes para el estudio de Machine Learning.

Tabajamos con 7 columnas para la fase de entrenamiento, ya que si trabajamos con mas columnas que tienen datos irrelevante se obtiene mayor procentaje de error.
 #   Column         Non-Null Count  Dtype  
---  ------         --------------  -----  
 0   Price          19237 non-null  int64  
 1   Levy           13418 non-null  float64
 2   Prod. year     19237 non-null  int64  
 3   Engine volume  17306 non-null  float64
 4   Mileage        19237 non-null  int64  
 5   Cylinders      19237 non-null  float64
 6   Airbags        19237 non-null  int64 

VErificamos si existen datos faltantes dentro de las columnas seleccionadas y las rellenamos con 0

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
Price		Levy	Engine volume	Mileage		Cylinders	Airbags
13328.0		1.0	1.3		91901.0		6.0		12.0
La precio del vehiculo es de 2008.83

Algoritmo de arboles:
Con los mismos valores el precio del vehiculo es de 2012

Agoritmo de red neuronal:
Con los mismos valores el precio del vehiculo es de 2010

COn los tres modelos se obtiene un precio de vehiculo entre 2008 y 2012, que se puede decir que tienen un valor promedio de 2010 que es el resultado de la red neuronal.


