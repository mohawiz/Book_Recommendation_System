Book Recommendation System with Cosine Similarity
This is a Python script that utilizes cosine similarity to recommend books based on their content.

Dependencies
This script requires the following Python libraries:

pandas (pd)
numpy (np)
sklearn.feature_extraction.text (TfidfVectorizer)
sklearn.metrics.pairwise (linear_kernel)
plotly.express (px) (optional, for data visualization)
Data
The script expects a CSV file containing book information, including:

bookID (integer) - Unique identifier for the book
title (string) - Title of the book
authors (string) - Author(s) of the book
average_rating (float) - Average rating of the book (optional)
Note: The script preprocesses the data by combining the title and authors columns into a single book_content column for vectorization.

Functionality
The script performs the following steps:

Imports libraries
Reads data from CSV file
(Optional) Visualizes data distribution (average rating, top authors)
Defines a function to add a new book to the dataset (optional)
Converts average_rating to a numeric data type
Creates a new column book_content by combining title and authors
Performs TF-IDF vectorization on book_content
Calculates cosine similarity between book vectors
Defines a function recommend_books that takes a book title as input and recommends the top 10 most similar books
Usage
Save the script as a Python file (e.g., book_recommender.py).
Place your book data CSV file in the same directory.
The script will print recommendations for a sample book title ("A Severed Head").
You can test the recommendation function with other book titles in the dataset:
Additional Notes
This is a basic implementation of a book recommendation system. You can further improve it by:
Including additional features like genre, description, or user ratings.
Implementing different similarity measures (e.g., Pearson correlation).
Building a user interface for interactive recommendations.
The optional data visualization using plotly.express can be used to explore the characteristics of your book data.
By following these steps and understanding the code, you can create your own book recommendation system using cosine similarity.
