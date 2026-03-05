# 🎵 SoundSense – Spotify Music Recommendation System

## 📌 Project Overview
SoundSense is a data science and machine learning project that builds a music recommendation system using the Spotify dataset.  
The system analyzes audio features of songs and suggests similar tracks based on user input.

The project is implemented in Python using data analysis, clustering techniques, and a content-based recommendation algorithm.

---

# 📊 Project Workflow

The project is organized into four main phases:

## 1️⃣ Data Loading
In this phase we load multiple Spotify datasets including:

- Main song dataset
- Genre dataset
- Artist dataset
- Year dataset

The data is explored and basic preprocessing is performed.

Key steps:
- Reading CSV files using **Pandas**
- Inspecting dataset structure
- Creating a **decade feature** from the year column

---

## 2️⃣ Exploratory Data Analysis (EDA)

In this phase we analyze patterns in the Spotify dataset.

Visualizations include:

- Distribution of songs by decade
- Evolution of audio features across years
- Loudness trends
- Top genres and their audio characteristics
- Word clouds for genres and artists

These analyses help understand how musical characteristics evolved over time.

---

## 3️⃣ Clustering Analysis

We applied multiple clustering algorithms to group songs based on their audio features:

### Algorithms Used
- **K-Means Clustering**
- **Hierarchical (Agglomerative) Clustering**
- **Spectral Clustering**

Because hierarchical and spectral clustering are computationally expensive, a **sample of 3000 songs** was used.

### Visualization
Clusters were visualized using **PCA dimensionality reduction**.

### Result
Among the tested methods, **Spectral Clustering produced better separated clusters**, capturing nonlinear relationships between songs.

These clusters represent different musical profiles based on Spotify audio features.

---

## 4️⃣ Recommendation System

A **content-based recommendation system** was implemented.

### How it works

1. The user inputs a song name and year.
2. The system retrieves its audio features.
3. A **mean feature vector** is computed.
4. **Cosine similarity** is used to find the most similar songs.

If the song is not present in the dataset, the system uses the **Spotify API (Spotipy)** to retrieve its features.

---

# ⚙️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Plotly
- Spotipy (Spotify API)
- Matplotlib / Seaborn

---

# 📂 Project Files

The repository contains the following notebooks:

- Data loading and preprocessing
- Exploratory data analysis
- Clustering experiments
- Recommendation system implementation

---

# ⚠️ Important Note

To correctly explore the entire project:

➡️ **Download all notebooks in this repository and run them sequentially.**

Some cells depend on previously executed steps, so running the full notebooks ensures correct execution.

---

# 🎯 Conclusion

This project demonstrates how machine learning techniques such as clustering and similarity analysis can be used to build an intelligent music recommendation system using Spotify audio features.

---

# 👨‍💻 Author

Rayen Bouazizi  
Data Science & Machine Learning Project
