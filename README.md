# Movie Recommendation System

Successfully developed an end-to-end Machine Learning project that implements a content-based movie recommendation system. This project demonstrates the full lifecycle of building a data driven application, from raw data processing to the deployment of a production-ready web service.

Deployed URL - <https://movie-recommendation-system-yuvraj.streamlit.app/>

## Project Overview

This application recommends movies by analyzing their metadata—specifically titles, overviews, genres, and taglines. By leveraging Natural Language Processing (NLP), the system converts these textual attributes into numerical representations to calculate similarity between films.

## Core Functionalities
### 1. Data Processing & NLP Pipeline
- Data Cleaning: Extensive data preparation performed, including handling duplicates, missing values, and filtering for relevant features.
- Text Preprocessing: A robust pipeline built to standardize the text data, including:
    - Lowercasing all text for consistency.
    - Removing punctuation using regular expressions.
    - Removing stop-words to eliminate noise.
    - Removing stop-words to eliminate noise.
- Vectorization: TF-IDF (Term Frequency-Inverse Document Frequency) utilized to transform processed text into vector representations.

### 2. Recommendation Logic
- Cosine Similarity: The core engine employs Cosine Similarity to measure the proximity between movie vectors. By calculating the angle between these vectors, the system accurately identifies movies with similar thematic content.
### 3. API & Deployment
- Backend: A REST API developed using FastAPI to serve the recommendation model, ensuring efficient communication between the model and the UI.
- Frontend: A user-friendly interface constructed using Streamlit, allowing users to search for movies and receive instant, personalized recommendations.

## Technical Stack
- Language: Python
- Machine Learning/NLP: Scikit-learn, NLTK, NumPy, Pandas
- Web Frameworks: FastAPI, Streamlit
- Data Source: TMDB API (used for fetching real-time movie metadata and posters)
- Deployment: GitHub