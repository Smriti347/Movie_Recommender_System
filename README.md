
# Movie Recommender System

This project is a content-based movie recommender system that suggests movies similar to a selected movie using the TMDB Movie Metadata dataset.

## Overview

The recommender system leverages Natural Language Processing (NLP) techniques to process movie descriptions, computes similarity scores using the TF-IDF (Term Frequency-Inverse Document Frequency) vectorization method, and employs cosine similarity to find and recommend movies similar to the selected title.

## Dataset

- **Source:** TMDB Movie Metadata Dataset  
- **Description:** The dataset contains metadata for thousands of movies, including titles, descriptions, genres, popularity, and more.  
- **Preprocessing:** Missing values in the descriptions are filled with empty strings.  

## Tech Stack

- Python  
- Pandas  
- NumPy  
- Scikit-Learn  
- NLTK  
- Streamlit  

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/movie-recommender-system
    cd movie-recommender-system
    ```
2. (Optional) Create a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # For Linux/Mac
    venv\Scripts\activate  # For Windows
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## How It Works

1. Load the dataset and preprocess it by filling missing values in descriptions.  
2. Convert movie descriptions into numerical vectors using TF-IDF.  
3. Calculate cosine similarity between the movie vectors.  
4. For a selected movie, recommend the top N movies with the highest similarity scores.  

## Usage

1. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```
2. Open the provided URL in your browser.  
3. Select a movie from the dropdown list and click the "Recommend" button.  
4. The app displays a list of similar movies.  

## Results

The system successfully recommends movies that are contextually similar based on the movie descriptions, providing a user-friendly interface for exploration.

## Future Enhancements

- Implement collaborative filtering to enhance recommendation accuracy.  
- Add user ratings and genre-based filtering.  
- Improve UI/UX with more visualizations.  


