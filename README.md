# Popularity-Based-Book-Recommendation-System

I developed a popularity-based book recommendation system using Google Colab, leveraging libraries like pandas, numpy, and matplotlib. The dataset was obtained from Kaggle.com, consisting of three CSV files: books.csv, ratings.csv, and users.csv. For this project, I utilized only the books and ratings CSV files.

![POPULARITY_BOOK_RECOMENDATION](https://github.com/ANSHPG/Popularity-Based-Book-Recommendation-System/assets/132222062/ce06315d-3de8-4acd-b1bc-1cc3ae8242e8)

The books dataset contained columns such as book title, author, year of publication, image, and ISBN, while the ratings dataset included columns like ISBN, user ID, and user rating. The initial steps involved data preprocessing, including handling null and duplicate values from both CSV files.

Next, I merged both datasets based on the ISBN column. However, before merging, I removed the user ID column from the ratings dataset. Then, I used group-by operations to determine the total number of reviews each book received based on the book title, as some books had multiple ISBNs.

With the total user ratings calculated, I proceeded to find the mean ratings each book received. Subsequently, I filtered out books that received 250 or more user ratings and arranged them in descending order based on mean ratings.

To showcase the top 50 recommended books, I utilized the head(50) function and displayed them. Through exploratory data analysis (EDA), I discovered that most people gave ratings of 1.0 to books, followed by a spike at 4.5.

For reference, I drew inspiration from IMDb's movie recommendation system, incorporating a similar formula, which I explained and implemented in the notebook. The entire project, along with explanations, is documented in a mind-map format and is publicly available for use.

The repository containing the project is owned by Anshuman Pattnaik and is accessible to all for public use.
