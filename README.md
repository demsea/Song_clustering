# Songs_clustering

# 🎧 Moosic - Playlist Generation with Clustering

**Moosic** is a startup revolutionizing the way we experience curated music. Each playlist is handcrafted by music experts to match a unique *mood* or *style*, but as user demand grows, so does the need to scale. This project explores the use of **Data Science** to automate the creation of playlists using **Spotify audio features** and **clustering algorithms**.

## 🚀 Project Objective

Moosic aims to enhance their playlist creation process by integrating machine learning techniques. Your mission: build a prototype that groups songs into clusters (i.e. playlists) based on their audio characteristics.

This first iteration uses:
- Spotify audio features (tempo, energy, danceability, etc.)
- **PCA** for dimensionality reduction
- **K-Means** clustering to generate playlists

The project also evaluates whether these audio features can truly capture the *mood* or *style* of a song — a question that's both subjective and essential for Moosic's brand.

---

## 🧠 Business Questions

- Can Spotify’s audio features identify “similar songs” based on human perception?
- Is K-Means an effective algorithm for playlist creation?
- What are the optimal preprocessing steps to enhance clustering?

---

## 🛠️ What I Did

### 1. **Data Preprocessing**
- Tested various **scalers/transformers** (e.g., StandardScaler, MinMaxScaler) to normalize audio features.
- Chose the most suitable transformation based on clustering performance.

### 2. **Dimensionality Reduction with PCA**
- Applied **Principal Component Analysis (PCA)** to reduce noise and improve clustering performance.
- Used **Cumulative Explained Variance** to retain 95% of the data's variance.
- Created a plot to visualize how many components were needed to reach the threshold.

### 3. **Clustering with K-Means**
- Evaluated optimal number of clusters using:
  - **Silhouette Score**
  - **Inertia (Elbow Method)**
- Selected **50 clusters** to serve as preliminary playlists.
- Assigned cluster labels to all tracks.

---

## 📊 Results

- Successfully clustered 5000 tracks into 50 distinct groups.
- Visualized clusters and key PCA insights with Radar chart.

