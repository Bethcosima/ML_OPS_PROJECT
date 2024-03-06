![Pandas](https://img.shields.io/badge/-Pandas-333333?style=flat&logo=pandas)
![Numpy](https://img.shields.io/badge/-Numpy-333333?style=flat&logo=numpy)
![Matplotlib](https://img.shields.io/badge/-Matplotlib-333333?style=flat&logo=matplotlib)
![Seaborn](https://img.shields.io/badge/-Seaborn-333333?style=flat&logo=seaborn)
![Scikitlearn](https://img.shields.io/badge/-Scikitlearn-333333?style=flat&logo=scikitlearn)
![FastAPI](https://img.shields.io/badge/-FastAPI-333333?style=flat&logo=fastapi)
![TextBlob](https://img.shields.io/badge/-TextBlob-333333?style=flat&logo=textblob)
![Render](https://img.shields.io/badge/-Render-333333?style=flat&logo=render)

<h1 align= center>PROYECTO INDIVIDUAL N°1<h1>
<h1 align= center>Machine Learning Operations</h1>
<p align=center><img src=https://www.edsrobotics.com/wp-content/uploads/2021/01/deep-learning.jpg><p>

<h1 align= left> Introducción</h1>
  
<p align= justify>En este proyecto se trata de realizar un modelo de ML el cual pretende crear una recomendación de videojuegos para usuarios. Durante el proyecto se realizaron trabajos de Data Engineer para obtener un Producto Minimamente Viable (MVP, por sus siglas en inglés) enfocado en consultar datos específicos y la recomendación de juegos similares a otros juegos dados por el usuario.

El proyecto tiene principalmente cómo objetivo desarrollar una API de manera que la empresa tenga disponibles los datos usando FastAPI de manera local y posteriormente deployando en render, así mediante este ultimo  se puedan realizar consultas.</p> 

<h1 align= left>Datasets</h1>
  
<p align = justify> Para poder llevar a cabo el desarrollo de este proyecto se proporcionaron 3 archivos de tipo JSON:
  
-<b>[output_steam_games.json](ETL-EDA/Archivos/output_steam_games.parquet)</b> En el cual podemos encontrar la información de los juegos como es el nombre, precio, fecha de lanzamiento, desarrolladora, etc.

-<b>[australian_users_items.json](ETL-EDA/Archivos/australian_users_items.parquet)</b> Aquí encontramos la ifnormación de los usuarios que utilizan estos juegos, así como el tiempo de juego.

-<b>[autralian_users_reviews.json](ETL-EDA/Archivos/australian_user_reviews.parquet)</b> En este archivo encontramos las recomendaciones de los usuarios, las reviews, ademas del id de usuario.

Los archivos anteriores se pueden encontrar en la carpeta de archivos dentro de la carpeta ETL/EDA, se decidió subirlos en formato parquet debido a que esto ahorraría espacio para posteriormente deployarlo en render o cualquier otra aplicación de hosting
</p>


<h1 align= left>Extracción, Transformaión y Carga (ETL)</h1>
<p align = justify>En esta etapa se llevó a cabo la extracción de los datasets antes mencionados, se llevó a cabo una limpieza en los datos y se hicieron tranformaciones necesarias como el cambio de tipo de dato en las columnas para posteriormente usarlas en la API. También se eliminaron columnas que no eran de nuestro interes en cada uno de los datasets con el fin de más adelante convertir los datasets en archivos parquet.</p>

<h1 align= left>Feature engineering</h1>

<p align = justify>Aquí se realizó el analisis de sentimientos con la librería de textBlob aplicandola a una de las columnas donde se encontraban los comentarios de los usuarios, siendo reviews.parquet el dataset a utilizado ya que fue el resultado del etl y contiene los datos necesarios para esta etapa. Podemos encontrar el notebook de esta seccion en el siguiente link: FE_API.ipynb.
También en esta parte se intento separar los dataset en solamente las columnas usadas, además podemos encontrar el desarrollo de las funciones para la api, antes de pasarlas a un archivo .py, pero este desarrollo se describe más adelante
</p>


<h1 align= left>Análisis Eploratorio de Datos (EDA)</h1>

<p align = justify>En esta parte del proyecto se realizó el análisis de los daset después de haber realizado el ETL, obteniendo una mejor visualziacion  de las variables. Con el fin de idenfiticar que variables serían necesarias para el modelo de Machine Learning</p>
[EDA](ML_OPS_PROJECT/ETL-EDA/EDA.ipynb)

<h1 align= left>Datasets</h1>
<p align = justify></p>

