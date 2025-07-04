# Recomendador de Películas - Proyecto Final

Este proyecto es una aplicación web interactiva que permite recomendar películas a partir de una búsqueda textual y múltiples filtros como géneros, idioma, país, actores y productoras. 

# Características principales

El proyecto está organizado de la siguiente manera:

Interfaz web desarrollada con Streamlit.
Recomendaciones basadas en similitud semántica utilizando TF-IDF y KNN.
Filtros interactivos para:
Actores principales
Director
Productoras
Géneros
Idiomas y países
Preprocesamiento de texto para mejorar la calidad de las búsquedas.
Integración con un notebook exploratorio para análisis y prototipado.


# Estructura del proyecto

```bash
├── app.py                 # Aplicación principal de Streamlit
├── explore.ipynb         # Notebook para análisis exploratorio y desarrollo del modelo
├── requirements.txt      # Requisitos del entorno (añadir si no existe)
├── data/                 # Carpeta para almacenar el dataset de películas
│   └── movies.csv        # Archivo con los datos limpios y enriquecidos
```

## Requisitos

**Prerrequisitos**

Python 3.9 o superior
Streamlit
Pandas
Scikit-learn
NLTK
Instala los requisitos ejecutando:

```bash
pip install -r requirements.txt
```

Si no tienes un archivo requirements.txt, puedes generarlo con:

```bash
pip freeze > requirements.txt
```


## Cómo ejecutar la app

Para ejecutar la aplicación, ejecuta el script app.py desde la raíz del directorio del proyecto:

```bash
python src/app.py
```

## Dataset

Se utiliza un dataset personalizado de películas que incluye:

Información textual: título, sinopsis, keywords, tagline.
Datos estructurados: actores principales, director, productoras, país, idioma y género.
La limpieza y vectorización se realiza con técnicas de procesamiento de lenguaje natural (NLP) y la similitud se calcula con un modelo KNN.

## Modelo de recomendación

Preprocesamiento:
Eliminación de duplicados
Lemmatización
Filtrado por POS (solo sustantivos, verbos y nombres propios)
Vectorización con TF-IDF
Cálculo de similitud usando KNN (NearestNeighbors)

## Autores

Iris Muñoz 
Loïc Barbera
Javier Gonzalez

## Licencia

Este proyecto se encuentra bajo licencia MIT, puedes usarlo y modificarlo libremente.