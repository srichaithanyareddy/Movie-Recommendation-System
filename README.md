🎬 Movie Recommendation System (Content-Based Filtering)

A Machine Learning project that recommends similar movies based on metadata such as genres, keywords, cast, director, and tagline using TF-IDF Vectorization and Cosine Similarity.

This system takes a movie name as input and suggests the top 30 most similar movies.

📌 Project Overview

Recommendation systems are widely used by streaming platforms to improve user engagement.

This project implements a Content-Based Recommendation System, where recommendations are generated based on similarities between movie attributes rather than user interaction history.

The model analyzes textual metadata and computes similarity scores to suggest relevant movies.

🧠 Approach

The project follows a structured machine learning workflow:

1️⃣ Data Collection

Dataset containing 4803 movies

Includes metadata such as genres, cast, director, keywords, and tagline

2️⃣ Data Preprocessing

Selected relevant features:

genres

keywords

tagline

cast

director

Handled missing values using fillna('')

Combined selected features into a single text column

3️⃣ Feature Extraction

Used:

TfidfVectorizer()


to convert textual data into numerical feature vectors.

4️⃣ Similarity Computation

Used:

cosine_similarity()


to compute similarity scores between movies.

5️⃣ Recommendation Logic

Accept user input

Find closest matching movie title using difflib

Retrieve similarity scores

Sort results in descending order

Display top 30 recommended movies

🛠️ Technologies Used

Python

NumPy

Pandas

Scikit-learn

difflib

Google Colab

📂 Dataset

4,803 movies

24 features

Metadata-based recommendation

CSV format

File used: movies.csv

▶️ How to Run (Google Colab)

Open the notebook in Google Colab.

Upload movies.csv using the file upload option.

Run all cells sequentially.

Enter your favorite movie name when prompted.

▶️ How to Run Locally

Clone the repository:

git clone https://github.com/your-username/movie-recommendation-system.git
cd movie-recommendation-system


Install dependencies:

pip install -r requirements.txt


Make sure movies.csv is in the project directory.

Run the notebook or convert it to a Python script.

📊 Example

Input:

Iron Man


Output:

1. Iron Man 2
2. The Avengers
3. Captain America
...

📈 Future Improvements

Include movie overview column for richer context

Implement Collaborative Filtering

Build a web interface using Streamlit

Deploy as a web application

Optimize similarity computation for large datasets

Integrate TMDB API for real-time movie data

🎯 Learning Outcomes

Understanding Content-Based Recommendation Systems

Text Feature Engineering

TF-IDF Vectorization

Cosine Similarity

Handling user input and fuzzy matching

👨‍💻 Author

Sri Chaithanya
B.Tech CSE (Data Science)
Aspiring Machine Learning Engineer
