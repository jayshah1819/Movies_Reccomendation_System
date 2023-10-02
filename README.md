# Movies_Reccomendation_System

Here's a summary of the code:
	Data Loading and Preprocessing:
The code starts by importing necessary libraries like Pandas, NumPy, and scikit-learn.
It reads a CSV file named "movies.csv" using pd.read_csv() and stores it in the variable movies_data.
It defines a set of selected features like genres, keywords, taglines, cast, and director.
Missing values in these features are filled with empty strings.
	Combining Features:
The selected features are combined into a single string named combined_features.
	TF-IDF Vectorization:
TfidfVectorizer() from sci-kit-learn is used to convert the combined features into TF-IDF vectors. This assigns a numerical value to each term based on its importance in the entire dataset.
	Cosine Similarity Calculation:
Cosine similarity is computed between the feature vectors using cosine_similarity().
	User Input:
The user is prompted to enter their favourite movie name.
	Finding Similar Movies:
The code finds the index of the user's favourite movie in the dataset and calculates similarity scores with all other movies.
	Recommendation:
The top 10 similar movies are selected (excluding the user's favourite movie itself).
The recommended movies along with their similarity scores are printed.
