# Content-Based Recommendation System

## Introduction
I implemented two recommendation algorithms: Content Filtering and Collaborative Filtering.

1. Content Filtering:

   - I created vector representations for each movie using TF-IDF.

   - I trained ridge regression models for each user to determine weights.

   - I constructed a linear regression model utilizing these weights to predict and recommend movie ratings.

2. Collaborative Filtering:

   - I utilized two approaches: item-item and user-user.

   - I calculated cosine similarity between items or users.

   - I implemented a KNN model by selecting K similar users/items to predict rating scores. 

## Environment Setup
1. Install Python libraries: `numpy`, `scikit-learn`,`pandas`.
2. Use data from the training and test sets to train the model.

## Libraries and Technologies
- **Programming Language:** Python
- **Main Libraries:** NumPy, scikit-learn,pandas
- **Technology:** Ridge Regression, TF-IDF Transformer

## Usage
1. Create a Content-Based object with training data and necessary parameters.
2. Call the `fit()` method to train the model.
3. Use the `RMSE()` method to evaluate performance on the test set.
4. Use the `recommend(user_id, top)` method to provide recommendations for a specific user.

## Performance Evaluation
- Utilize Root Mean Squared Error (RMSE) to assess the accuracy of the model on the test set.
- Evaluate performance by calculating Precision and Recall for recommendation tasks.

## Data
The data used includes user information (age, gender, occupation) and their ratings for items. This data is split into training and test sets.

## Conclusion
This project provides a foundation for building a recommendation system using the Content-Based approach. The model has been trained and evaluated on real-world data to ensure good performance on recommendation tasks.
