# Spotify Genre Prediction

A machine learning notebook that predicts a song's genre from its audio features, built for ECS171.

## Overview

The notebook (`ECS171_spotify_genre_prediction_models.ipynb`) loads a Spotify songs dataset, groups its 114 raw genres into 9 broader classes (Rock, Electronic, Pop, Classical, Jazz, R&B, Latin, Metal, Country), and trains two classifiers on the same train/test split:

- **Random Forest**
- **Logistic Regression**

Both models are evaluated with accuracy, balanced accuracy, classification reports, and confusion matrices, plus feature-importance analysis.

## Features used

`danceability`, `energy`, `loudness`, `speechiness`, `acousticness`, `instrumentalness`, `liveness`, `valence`, `tempo`, `duration_ms`, `popularity`

## Data

The dataset is loaded directly from a public URL in the notebook, so no manual download is needed:
`https://raw.githubusercontent.com/bohkuri/spotify_songs_dataset/main/dataset.csv`

## Requirements

- Python 3.12
- `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

Install them with:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Usage

Open the notebook in Jupyter (or VS Code) and run the cells top to bottom:

```bash
jupyter notebook ECS171_spotify_genre_prediction_models.ipynb
```

The first cell handles all data loading and preprocessing; the remaining cells train and evaluate each model.
