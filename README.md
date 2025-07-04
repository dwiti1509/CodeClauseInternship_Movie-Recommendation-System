# 🎬 Movie Recommender System

This project is a **Content-Based Movie Recommender System** built using **Python** and deployed via **Streamlit**. It suggests movies similar to the one selected by the user based on a precomputed similarity score. The recommendations include movie titles and official posters fetched in real time using the **TMDB API**.

---

## 📌 Objective

The main goal of this project is to help users discover movies similar to the ones they already enjoy. By analyzing the features of a given movie, the system returns a list of top 5 most similar movies along with their posters, providing a smooth and engaging experience.

---

## ✅ Features

- 🔍 Select a movie from the dropdown list
- 🤖 Get 5 recommended movies based on similarity
- 🖼️ View posters of recommended movies using the **TMDB API**
- ⚡ Fast response with precomputed similarity scores
- 🌐 Interactive user interface built with **Streamlit**

---

## 🧠 How It Works

1. **Data Preparation:**
   - A dataset of movies is preprocessed and stored as a dictionary (`movie_dict.pkl`)
   - A similarity matrix is calculated using cosine similarity and saved as `similarity.pkl`

2. **Recommendation Engine:**
   - When a user selects a movie, the app:
     - Finds the movie index
     - Retrieves similarity scores
     - Sorts them to find the top 5 closest matches
     - Fetches posters from **TMDB API** using each movie's ID

3. **Poster Fetching:**
   - The **TMDB API** is used to fetch the official poster for each recommended movie using the movie's TMDB ID.

---

## 🛠️ Technologies Used

- **Python**
- **Streamlit** – for building the web application
- **Pandas** – for data manipulation
- **Pickle** – for storing preprocessed data
- **Requests** – to make API calls to TMDB
- **TMDB API** – for fetching movie posters

---


## ▶️ Run the App

To run the Streamlit application locally:

```bash
streamlit run app.py
```

## Once the app launches, open your browser and go to:
http://localhost:8501

## Sample Output:

![select_movie](https://github.com/user-attachments/assets/843c0a73-2e93-4715-834f-3ba3ea60153c)
 
## Recommended Results:

 ![recommendations](https://github.com/user-attachments/assets/94f62f2a-44e5-4465-add6-d00cc4e5e8de)




