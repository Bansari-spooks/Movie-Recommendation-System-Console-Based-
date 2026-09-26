# 🎬 Movie Recommendation System

A **content-based movie recommendation system** built with Python that recommends similar movies based on a movie title entered by the user.

The system combines movie metadata, **TF-IDF Vectorization**, and **Cosine Similarity** to generate relevant recommendations dynamically.

## ⭐ Recommendation Flow

The core of the project is the **interactive recommendation pipeline**. The user simply enters a movie name, and the system processes it through the following steps:

```text
                    🎬 USER INPUT
                         │
                         ▼
              Enter Movie Title
                         │
                         ▼
                🔎 Movie Matching
                         │
                         ▼
             📝 Extract Movie Features
        (Genres • Keywords • Cast • Director
                 • Overview)
                         │
                         ▼
              🧠 TF-IDF Vectorization
                         │
                         ▼
             📐 Cosine Similarity
                         │
                         ▼
          📊 Calculate Movie Similarity
                         │
                         ▼
             🔝 Rank Similar Movies
                         │
                         ▼
             🎥 RECOMMENDATIONS
```

### 🔥 How It Works

**1. 🎬 User enters a movie**

The final interactive cell asks the user to enter a movie title.

```text
Enter the movie name: Avatar
```

**2. 🔎 Movie is identified**

The system searches the dataset for the entered movie and handles title matching to identify the appropriate movie.

**3. 📝 Movie features are collected**

Relevant information such as **overview, genres, keywords, cast, and director** is used to represent the movie.

**4. 🧠 TF-IDF converts text into numerical features**

The combined textual information is transformed into numerical vectors using **TF-IDF Vectorization**.

**5. 📐 Similarity is calculated**

The system compares the selected movie against other movies using **Cosine Similarity**.

**6. 🔝 Similar movies are ranked**

Movies are ranked according to their similarity score.

**7. 🎥 Recommendations are displayed**

The system returns the **most similar movies** as recommendations based specifically on the movie entered by the user.

> **Input one movie → Analyze its features → Compare with the dataset → Return similar movies**

---

## ✨ Key Features

* 🎬 Interactive movie input
* 🔎 Movie title matching
* 🧠 TF-IDF-based feature representation
* 📐 Cosine similarity
* 🎥 Content-based recommendations
* 🔝 Similar movie ranking
* 📊 Metadata-based movie comparison

## 🛠️ Technologies Used

* **Python**
* **Pandas** — Data loading and manipulation
* **NumPy** — Numerical operations
* **Scikit-learn** — TF-IDF and cosine similarity
* **Difflib** — Movie title matching

## 📊 Dataset

The system uses movie metadata including:

* Movie title
* Overview
* Genres
* Keywords
* Cast
* Director
* Ratings and other available attributes

These features provide the textual information required to determine movie similarity.

## 🚀 How to Run

### Install Dependencies

```bash
pip install pandas numpy scikit-learn
```

### Run the Project

```bash
python bansarinimbalkar_project_2.py
```

Enter a movie title when prompted:

```text
Enter the movie name: Avatar
```

The system then generates recommendations based on the similarity of **Avatar** to other movies in the dataset.

## 🎯 Project Objective

The project demonstrates how **content-based filtering and NLP techniques** can be used to build an interactive recommendation system where recommendations are generated dynamically from a user's movie selection.

## 🔄 Core Pipeline

**User Movie Input → Movie Matching → Feature Extraction → TF-IDF → Cosine Similarity → Similarity Ranking → Movie Recommendations**

## 🔮 Future Enhancements

* Streamlit web interface
* Movie posters and additional metadata
* Improved title search
* Genre-based filtering
* Interactive recommendation interface
* Online deployment

## 👨‍💻 Author

**Bansari Nimbalkar**

Computer Science & Engineering (Data Science)

---

⭐ If you find this project useful, consider giving the repository a star.
