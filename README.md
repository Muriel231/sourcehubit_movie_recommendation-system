# sourcehubit_movie_recommendation-system

## Objective
The goal of this task was to develop a Movie Recommendation System that suggests movies to users based on their preferences or past ratings. The system should utilize collaborative filtering or content-based filtering techniques and be built using Python with libraries such as pandas, NumPy, and optionally scikit-learn or Surprise. The MovieLens dataset was used for model training and evaluation.

## Tools & Technologies Used
Programming Language: Python

Libraries: pandas, NumPy, scikit-learn

Dataset: MovieLens (latest-small version)

## Methodology
Step 1: Data Loading and Preprocessing

Loaded ratings.csv and movies.csv from the MovieLens dataset.

Merged data to form a user-item matrix.

Filled missing ratings with zeros to prepare for similarity computation.

Step 2: Collaborative Filtering

Implemented Item-Based Collaborative Filtering.

Used Cosine Similarity (from scikit-learn) to compute similarity between movies.

Predicted user ratings based on weighted averages of similar items.

Step 3: Generating Recommendations

For a given user, identified movies not yet rated.

Ranked movies based on predicted scores.

Recommended the top N movies.

Step 4: Model Evaluation

Performed an 80-20 split of the dataset into training and test sets.

Predicted ratings on the test set.

Evaluated performance using Root Mean Squared Error (RMSE).

RMSE on Test Set: 0.9219

## Sample Output
Top 5 movie recommendations for User 1: ['Jumanji (1995)', 'Waiting to Exhale (1995)', 'Father of the Bride Part II (1995)', 'Sabrina (1995)', 'Tom and Huck (1995)']

Top 5 movie recommendations for User 5: ['Jumanji (1995)', 'Grumpier Old Men (1995)', 'Waiting to Exhale (1995)', 'Father of the Bride Part II (1995)', 'Heat (1995)']

Top 5 movie recommendations for User 10: ['Toy Story (1995)', 'Jumanji (1995)', 'Grumpier Old Men (1995)', 'Waiting to Exhale (1995)', 'Father of the Bride Part II (1995)']

## Conclusion
The system effectively recommends movies using item-based collaborative filtering. An RMSE of 0.9219 on the test set indicates the model's predictions are fairly accurate on unseen data, particularly for a simple model built from scratch without advanced tuning.

The project fulfills the objective of building a functional movie recommendation system using Python, pandas, NumPy, and scikit-learn, utilizing the MovieLens dataset.

