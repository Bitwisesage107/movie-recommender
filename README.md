# Movie Recommendation System

This is a content-based movie recommendation web application built using Python and Streamlit. It recommends similar movies based on a selected movie's metadata such as genres, cast, crew, and keywords. Movie posters are retrieved using the TMDB API.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features](#features)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Deployment](#deployment)
  - [Deploying on Heroku](#deploying-on-heroku)
  - [Deploying on Streamlit Cloud](#deploying-on-streamlit-cloud)
- [Folder Structure](#folder-structure)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

This project is a content-based recommendation engine. It suggests top 5 movies similar to the one selected by the user. The backend uses cosine similarity over processed metadata from the TMDB 5000 Movie Dataset. The frontend is implemented using Streamlit for a fast and interactive user interface.

## Dataset

The dataset used is the [TMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata), which includes:
- Movie metadata (title, genres, keywords, cast, crew, etc.)
- Ratings, popularity, and other information

The dataset is preprocessed and stored in two pickle files:
- `movie_dict.pkl`: Dictionary containing movie data
- `similarity.pkl`: Precomputed cosine similarity matrix

## Features

- Recommends five similar movies based on content
- Uses TMDB API to display posters of recommended movies
- Responsive web interface using Streamlit
- Ready for deployment on Heroku or Streamlit Cloud

## Setup and Installation

Follow these steps to run the project locally:

### 1. Clone the Repository

```bash
git clone https://github.com/Bitwisesage107/movie-recommender.git
cd movie-recommender
