# Book Recommednation Model 

A simple yet effective book recommendation system using K-Nearest Neighbors (KNN) algorithm!
Given a book title, it recommends 5 similar books based on feature similarity.


# Goal:

Suggest books similar to a user's input book title.

# How it works:
1) Looks up the feature vector of the given book.
2) Uses a pre-trained KNN model to find the nearest neighbors (similar books).
3) Returns the top 5 closest books along with their similarity scores.

#Tech Stack
1) Python

2) Pandas (for data handling)

3) Scikit-learn (for KNN modeling)

# Project structure 
├── Book Recommendation System.ipynb  # Main notebook
├── README.md                         # Project documentation (this file)
└── requirements.txt                  # Python libraries required (optional)


#`How to use 

Step 1 : Prepare your dataset
         Ensure you have a DataFrame (df) with:
         1) Index: Book titles
         2) Values: Feature vectors (like genres, keywords, embeddings, etc.)

Step 2 : Train or load a KNN model
         Example:from sklearn.neighbors import NearestNeighbors
         model = NearestNeighbors(metric='euclidean', algorithm='auto')
         model.fit(df.values)

Step 3 : Use the get_recommends function
         books = get_recommends("Where the Heart Is (Oprah's Book Club (Paperback))")
         print(books)

Step 4 : Test the recommender system
         Run the test_book_recommendation() function to validate the output. 

# Example Output
[
  "Where the Heart Is (Oprah's Book Club (Paperback))",
  [
    ["I'll Be Seeing You", 0.80],
    ["The Weight of Water", 0.77],
    ["The Surgeon", 0.77],
    ["I Know This Much Is True", 0.77],
    ["The Lovely Bones: A Novel", 0.72]
  ]
]
# Features
1) Accurate similarity matching based on pre-computed features.

2) Easy-to-understand code structure.

3) Basic testing to validate recommendations.

4) Supports extension to larger datasets or more advanced models.

#Future Improvements
1) Improve feature engineering (use embeddings from book descriptions or reviews).

2) Use cosine similarity for better distance metrics.

3) Build a simple Streamlit app for interactive recommendations.

4) Add genre-based filtering or popularity-based boosting.

#Acknowledgements
1) Scikit-learn

2) Pandas

3) Goodbooks-10k Dataset (if you later train on it)

