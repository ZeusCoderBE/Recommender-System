# Recommender System

## Introduction

### Environment Setup
1. Install Python libraries: `numpy`, `scikit-learn`,`pandas`.
2. Use data from the https://www.kaggle.com/datasets/prajitdatta/movielens-100k-dataset.

### Data
The data used includes user information (age, gender, occupation),movies(Title,Genre) and their ratings for movies. This data is split into training(ua.base) and test(ua.test) sets.

### I implemented two recommendation algorithms: Content Filtering and Collaborative Filtering.

1. Content Filtering:

   - I created a vector representation for each movie using TF-IDF.

   - I trained a ridge regression model for each user to learn the weights.

   - I used these weights to predict and recommend movie ratings.

2. Collaborative Filtering:

   - I utilized two approaches: item-item and user-user.

   - I calculated cosine similarity between items or users.

   - I implemented a KNN model by selecting K similar users/items to predict rating scores. 

### Libraries and Technologies
- **Programming Language:** Python
- **Main Libraries:** NumPy, scikit-learn,pandas
- **Model:** Ridge Regression, TF-IDF Transformer,KNN User-User,KNN Item-Item

### Performance Evaluation
- Utilize Root Mean Squared Error (RMSE) to assess the accuracy of the model on the test set.

### Development Orientation 
- I will use a hybrid method between collaborative filtering and content filtering. The idea is that after building two algorithms, collaborative filtering and content filtering, use these two models to predict ratings for the test set. Then I will add the average rating of the two predicted results and then suggest it to the user

### Conclusion
- This project provides a foundation for building a recommendation system using the Content-Based and Collaborative Filtering approach . The model has been trained and evaluated on real-world data to ensure good performance on recommendation tasks.
