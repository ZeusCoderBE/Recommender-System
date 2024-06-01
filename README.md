# Recommender System

## Introduction

### Environment Setup
1. Install Python libraries: `numpy`, `scikit-learn`,`pandas`.
2. Use data from the https://www.kaggle.com/datasets/prajitdatta/movielens-100k-dataset.

### Data
The data used includes user information (age, gender, occupation),movies(Title,Genre) and their ratings for movies. This data is split into training(ua.base) and test(ua.test) sets.
### The main idea of the two algorithms Content Filtering and Collaborative Filtering
- Content Filtering :Suggest items based on the user's profile or based on the content/attributes of items similar to items the user has selected in the past.
  
![image](https://github.com/ZeusCoderBE/Recommender-System/assets/117000361/2714e86a-b43a-4bc2-b9ba-fc125739931e)

- Collaborative Filtering: Suggest items based on similarity between users and/or items. It can be understood that this is a way to suggest a user based on users with similar behavior.

![image](https://github.com/ZeusCoderBE/Recommender-System/assets/117000361/ed58ed37-ef56-4d87-bd19-38f33bcfa057)


### I implemented two recommendation algorithms: Content Filtering and Collaborative Filtering.

1. Content Filtering:

    - I created a vector representation for each movie using TF- IDF (item profiles). 

    - I trained a ridge regression model for each user to learn the weights(user profiles).

    - I used  item profiles and user profiles to predict and recommend movie ratings.

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
