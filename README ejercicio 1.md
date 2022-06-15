# ejerciciosJorge Carlos Pabon Sueldo

CONTEXTO DE PROBLEMA
Bob ha comenzado su propia empresa de telefonía móvil. Quiere dar una pelea dura a las grandes empresas como Apple, Samsung, etc.

No sabe cómo estimar el precio de los móviles que fabrica su empresa. En este competitivo mercado de telefonía móvil no se puede simplemente asumir cosas. 
Para resolver este problema, recopila datos de ventas de teléfonos móviles de varias empresas.

Bob quiere averiguar alguna relación entre las funciones de un teléfono móvil (p. ej., RAM, memoria interna, etc.) y su precio de venta. 
Pero no es tan bueno en Machine Learning. Así que necesita tu ayuda para resolver este problema.

En este problema, no tiene que predecir el precio real, sino un rango de precios que indica qué tan alto es el precio

DATASET
Puede descargar el dataset aqui: https://neuraldojo.org/media/mobile/archive.zip

El dataset esta constituido por las siguientes columnas:

 #   Column         Non-Null Count  Dtype  
---  ------         --------------  -----  
 0   battery_power  2000 non-null   int64  
 1   blue           2000 non-null   int64  
 2   clock_speed    2000 non-null   float64
 3   dual_sim       2000 non-null   int64  
 4   fc             2000 non-null   int64  
 5   four_g         2000 non-null   int64  
 6   int_memory     2000 non-null   int64  
 7   m_dep          2000 non-null   float64
 8   mobile_wt      2000 non-null   int64  
 9   n_cores        2000 non-null   int64  
 10  pc             2000 non-null   int64  
 11  px_height      2000 non-null   int64  
 12  px_width       2000 non-null   int64  
 13  ram            2000 non-null   int64  
 14  sc_h           2000 non-null   int64  
 15  sc_w           2000 non-null   int64  
 16  talk_time      2000 non-null   int64  
 17  three_g        2000 non-null   int64  
 18  touch_screen   2000 non-null   int64  
 19  wifi           2000 non-null   int64  
 20  price_range    2000 non-null   int64  

De los cuales se debe seleccionar los los datos que no sean relevantes para el estudio de Machine Learning, todos los datos son de tipo numerico 
por lo cual no se necesita cambiar el tipo de datos.

Requerimiento y librerias:
1. importamos los archivos creados en excel con la extension .csv (from  google.colab import files)
2. importamos las librerias pandas para leer archivos (import pandas as pd)
3. importamos matplotlib para mostrar graficas(import matplotlib.pyplot as plt)
4. importamos sklearn para hacer predicciones en modelo lineal (sklearn.linear_model import LinearRegression)
5. importamos numpy para mostrar el error (import numpy as np from sklearn.metrics import mean_squared_error)
6. importamos el arbol de decision de maching learning (import tree)
7. importamos neural_network  para clasificar los datos(.neural_network import MLPClassifier)





