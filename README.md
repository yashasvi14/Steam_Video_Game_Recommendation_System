# Game Recommendation System

This project implements a hybrid recommendation system for video games using both Collaborative Filtering and Content-Based Filtering techniques.

## Project Overview

The system recommends games to users based on three methodologies:
1. **Collaborative Filtering**: Identifies games liked by similar users based on user interactions.
2. **Content-Based Filtering**: Recommends games that have similar content attributes (e.g., genre, description) to those liked by the user.
3. **Hybrid Technique**: Combines collaborative and content-based filtering to provide comprehensive recommendations.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn

## Dataset

The system uses four datasets:
1. **recommendations_df**: Contains user reviews: whether the user recommends a product. The table represents a many-many relation between a game entity and a user entity
2. **games_df**: Contains information on ratings, pricing in US dollars $, release date, etc.
3. **games_metadata_df**: Contains game metadata, including tags, descriptions, and app IDs.
4. **users_df**: Contains user profiles' public information: the number of purchased products and reviews published

The dataset is sourced from Kaggle avaialble here [Game Recommendations on Steam](https://www.kaggle.com/datasets/antonkozyriev/game-recommendations-on-steam)

Recommendation and user datasets needs to be downloaded from Kaggle since the files are large

## Functions

### 1. `get_knn_recommendations`
   - Finds users similar to the given user ID 

### 2. `get_content_based_recommendations`
   - Returns similar games based on the content attributes of a specific game title.

### 3. `get_hybrid_recommendations`
   - Combines the outputs from collaborative and content-based filtering to suggest games to users by checking for similarities in both user preferences and game content.

