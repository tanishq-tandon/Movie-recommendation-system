
# Movie Recommendation System 🎥🍿

## 📋 Project Overview

This project is a **content-based Movie Recommendation System** built using Python. It utilizes machine learning techniques to recommend movies similar to the one selected by the user. The system is powered by the **TMDb 5000 Movie Dataset** and demonstrates data preprocessing, feature extraction, and similarity computation.

---

## 🛠️ Features
- Provides top 5 movie recommendations based on a selected movie.
- Processes movie metadata (genres, keywords, cast, crew, and overview).
- Implements **cosine similarity** for recommendation.
- Uses stemming and vectorization for efficient text processing.

---

## 📂 Project Structure

```
Movie-Recommendation-System/
├── tmdb_5000_movies.csv       # Dataset containing movie metadata
├── tmdb_5000_credits.csv      # Dataset containing cast and crew details
├── Movie-recommendation-system.ipynb  # Jupyter Notebook with the implementation
├── movie_dict.pkl             # Pickled movie data for deployment
├── similarity.pkl             # Pickled similarity matrix
└── README.md                  # Documentation for the project
```

---

## 🧰 Technologies Used

- **Programming Language**: Python
- **Libraries**: 
  - `pandas` - Data manipulation
  - `numpy` - Numerical computations
  - `sklearn` - Machine learning and text processing
  - `nltk` - Natural Language Processing (NLP)

---

## 📈 Methodology

1. **Data Loading**: Merged movie and credits datasets for a complete view.
2. **Data Preprocessing**:
   - Removed missing values and duplicates.
   - Extracted relevant features (genres, cast, crew, etc.).
3. **Feature Engineering**:
   - Combined multiple attributes into a single `tags` column.
   - Applied stemming and vectorization.
4. **Similarity Computation**:
   - Transformed text data into vectors using `CountVectorizer`.
   - Calculated similarity using `cosine_similarity`.
5. **Recommendation**:
   - Designed a function to fetch the top 5 similar movies based on the selected movie.

---

## ⚙️ How to Run the Project

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/Movie-Recommendation-System.git
   cd Movie-Recommendation-System
   ```

2. **Install Dependencies**:
   Make sure you have Python installed. Then, install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```
   *(Create a `requirements.txt` with dependencies like `pandas`, `numpy`, `scikit-learn`, and `nltk`.)*

3. **Run the Notebook**:
   Open the Jupyter Notebook:
   ```bash
   jupyter notebook Movie-recommendation-system.ipynb
   ```

4. **Test Recommendations**:
   - Replace the movie title in the `recommend()` function to see recommendations for different movies.

---

## 🌟 Example Output

```python
>>> recommend('Avatar')

1. Pirates of the Caribbean: At World's End
2. Guardians of the Galaxy
3. Alien
4. Star Trek Into Darkness
5. Gravity
```

---

## 🚀 Future Enhancements

- Incorporate **user-based collaborative filtering** for better personalization.
- Build a web interface using **Flask** or **Streamlit** for user interaction.
- Enhance the dataset with more recent movies.

---

## 🏗️ Contributing

Feel free to fork this repository, make improvements, and submit pull requests. Contributions are always welcome! 

---

## 📄 License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

---

## 🙋‍♂️ Contact

For queries or suggestions, reach out to me at [tanishqtandon10a@gmail.com](mailto:tanishqtandon10a@gmail.com).  
You can also find me on [LinkedIn](https://www.linkedin.com/in/tanishq-tandon-a140a132a).
