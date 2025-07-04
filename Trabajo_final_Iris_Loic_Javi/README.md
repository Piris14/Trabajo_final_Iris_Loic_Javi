# Movie Recommender – Final Project

This project is an interactive web application that recommends movies based on a free-text search and multiple filters such as genre, language, country, actors, and production companies.

# Key Features

The project is organized as follows:

- Web interface built with Streamlit  
- Recommendations based on semantic similarity using TF-IDF and KNN  
- Interactive filters for:  
  - Main actors  
  - Director  
  - Production companies  
  - Genres  
  - Languages and countries  
- Text preprocessing to improve search quality  
- Integration with an exploratory notebook for analysis and prototyping

# Project Structure

```bash
├── app.py                 # Main Streamlit application
├── explore.ipynb         # Notebook for exploratory analysis and model development
├── requirements.txt      # Environment dependencies (add if not present)
├── data/                 # Folder containing the movie dataset
│   └── movies.csv        # Cleaned and enriched data file
```

# Requirements

Python 3.9 or higher
Streamlit
Pandas
Scikit-learn
NLTK
Install the dependencies by running:

```bash
pip install -r requirements.txt
```

If you don't have a requirements.txt file, you can generate one with:

```bash
pip freeze > requirements.txt
```


## How to Run the App

To run the application, execute the app.py script from the root directory of the project:

```bash
python src/app.py
```

## Dataset

A custom movie dataset is used, which includes:

Textual information: title, overview, keywords, tagline
Structured data: main actors, director, production companies, country, language, and genre
Cleaning and vectorization are performed using natural language processing (NLP) techniques, and similarity is calculated using a KNN model.

## Recommendation Model

Preprocessing steps:

Duplicate removal
Lemmatization
POS filtering (only nouns, verbs, and proper nouns)
Vectorization with TF-IDF
Similarity calculation using KNN (NearestNeighbors)

## Authors

Iris Muñoz 
Loïc Barbera
Javier Gonzalez

## License

This project is licensed under the MIT License — you are free to use and modify it.