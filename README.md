# Sistema de recomendacion Collaborative Filtering con KNN
Sistema de Recomendación de Películas con Collaborative Filtering y KNN

Este proyecto implementa un sistema de recomendación de películas utilizando filtrado colaborativo basado en usuarios (User-Based Collaborative Filtering) con el algoritmo KNN (K-Nearest Neighbors). Está desarrollado en Python y permite predecir películas que pueden gustar a un usuario según los gustos de otros usuarios similares.

Contenido del proyecto:

-Limpieza y preprocesamiento de datos.
-Análisis exploratorio de datos (EDA).
-Generación de la matriz usuario-película.
-Entrenamiento del modelo KNN.
-Recomendaciones personalizadas.
-Función interactiva para que el usuario califique 5 películas y reciba sugerencias.

Estructura del proyecto:

Carpeta data: contiene los archivos de datos (ratings, movies, tags, etc.).

-Carpeta notebooks: contiene los análisis en Jupyter.
-Carpeta src: scripts reutilizables como el modelo y la lógica de recomendación.
-Archivo README.md: documentación general del proyecto.

Cómo funciona:

Se cargan los datos desde archivos CSV.
Se filtran películas y usuarios con poca actividad para reducir ruido.
Se construye una matriz de ratings con usuarios como filas y películas como columnas.
Se entrena un modelo KNN con distancia del coseno.
El usuario interactúa puntuando 5 películas y el sistema le recomienda otras 5 basadas en usuarios similares.

Requisitos:

Python 3.8 o superior
pandas
numpy
scikit-learn
seaborn o matplotlib

Uso:

Ejecuta el archivo principal recomendador.py para iniciar el sistema de recomendación interactivo. También puedes usar un notebook para explorar el análisis paso a paso.
Ejemplo de interacción:

Ingresa el movieId de la película #1: 1
¿Qué puntuación le das a 'Toy Story (1995)'? 5

Películas recomendadas:
The Lion King (1994)
Monsters, Inc. (2001)
Finding Nemo (2003)
...

Notas adicionales:

El proyecto trabaja con un subconjunto filtrado de los datos originales para mejorar el rendimiento.
Se utiliza la distancia del coseno como métrica de similitud por ser más robusta frente a la dispersión de los ratings.

Autor:

Lauren Deleanu
Proyecto académico y personal de aprendizaje en sistemas de recomendación.

Licencia:

Este proyecto está bajo la licencia MIT. Puedes usar, modificar y compartir libremente el código.
