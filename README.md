# 🎬 Movie Recommendation System
---

## 📌 Project Overview

**The Movie Recommendation System** is a machine learning-based project designed to help movie lovers discover movies they are likely to enjoy. By analyzing movie genres and user ratings, the system suggests relevant movies based on what you like and what people with similar tastes have rated highly.

To improve recommendation quality, the project implements **multiple recommendation techniques** including:
  - Content-Based Filtering (Genres, TF-IDF + Cosine Similarity)
  - Item-Based Collaborative Filtering (User Ratings + Cosine Similarity)
  - Hybrid Recommendation (Collaborative + Content-Based)

Users can compare performance through RMSE scores against a baseline. The project also includes a Gradio-based interactive web interface where users can select a movie or enter a user ID and instantly receive recommendations.

This system aims to:  
- ✅ Help users discover movies faster  
- ✅ Personalize suggestions based on ratings  
- ✅ Provide data-driven recommendations  

---

## ✨ Features  
- 🎥 Recommends movies based on genres and user ratings  
- 🍿 User-friendly **Gradio Web App** with four tabs  
- 📊 Performance evaluation using **RMSE vs. baseline**  
- 🔎 Includes **content-based, collaborative and hybrid** recommenders  
- ☁️ Runs easily in **Google Colab**  

---

## 🛠 Tech Stack  
- **Programming Language:** Python  
- **Libraries & Tools:**  
  - Pandas, NumPy, Scikit-learn  
  - Gradio (for the interactive interface)  
  - Google Colab (for running the notebook)  

---

## 📂 Dataset  
- **Source:** [MovieLens Latest Small](https://grouplens.org/datasets/movielens/latest/) – GroupLens Research  
- **Size:** ~100,000 ratings from 610 users on ~9,700 movies  
- **Features:**  
  - Ratings: userId, movieId, rating, timestamp  
  - Movies: movieId, title, genres  

---

## ➡️ Project Workflow

Dataset --> Data Loading --> Content-Based Filtering --> Collaborative Filtering --> Hybrid Model --> Evaluation (RMSE) --> Deployment (Gradio)

---

## ⚙️ Installation & Setup

1. **Open the Notebook in Google Colab**
    - Upload `Movie_Recommendation_System.ipynb` to [Google Colab](https://colab.research.google.com/), or open it directly from GitHub.

2. **Run All Cells**
    - Run the cells from top to bottom. The first cell installs Gradio and downloads the dataset automatically.

3. **Launch the App**
    - Run the last cell and open the Gradio link that appears, or use the interface shown inside the notebook.

---

## 🖥️ How to Use

Enter your input in the Gradio interface, click **Recommend**, and get your results.

| Tab | You enter | You get |
|---|---|---|
| By genre | A movie name | Movies with similar genres |
| Similar movies | A movie name | Movies that people with similar tastes also liked |
| For a user | A user ID (1 to 610) | That user's top-rated movies and personalized picks with predicted ratings |
| Hybrid | A user ID and an `alpha` value | Picks that combine ratings and genres |

---

## 🖼️ Sample Output

<img width="1229" alt="Sample output" src="sample_output.png" />
