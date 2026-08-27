# DataScience-Lab5

Clasificación de tweets de desastre (dataset Kaggle *NLP with Disaster Tweets*).

## Descripción de los datos

El archivo train.csv tiene 7 613 tweets y 5 columnas: id (identificador), keyword (palabra
clave del tweet, opcional), location (ubicación declarada por el autor, opcional), text (el
mensaje del tweet) y target (la etiqueta a predecir: 1 si habla de un desastre real, 0 si
no).

text y target están completos. A keyword le falta menos del 1 por ciento de los valores y a
location le falta la tercera parte. Las clases están algo desbalanceadas pero no mucho: 57
por ciento no son desastres y 43 por ciento sí.

Los tweets son cortos (mediana de 15 palabras). Poco más de la mitad trae un enlace, uno de
cada cuatro menciona a otra cuenta y uno de cada cinco usa hashtag; no hay emojis porque el
dataset ya viene depurado. El texto del tweet es la información principal para clasificar.
keyword también es útil porque la proporción de desastres cambia mucho según la palabra
clave. location aporta poco: son 3 341 valores escritos a mano y sin normalizar.

Hay 110 tweets con texto repetido y 18 textos idénticos con etiquetas contradictorias, que
habrá que tratar en el preprocesamiento.
