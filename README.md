# 🎌 Ani Compass

> A machine learning–based anime recommendation system that helps users discover anime based on their preferences.

<p align="center">
  <img src="./ani-compass/project-overview.webp" alt="Project Overview" width="900">
</p>

---

## ✨ Features

- 🎯 Content-based anime recommendations
- 🧠 K-Means clustering
- 📝 TF-IDF synopsis vectorization
- 🔍 Fuzzy search for typo handling
- ⚡ Fast recommendations without user history

---

# 🏗️ System Architecture

```mermaid
flowchart LR
    A[Anime Dataset] --> B[Data Cleaning]
    B --> C[TF-IDF Vectorization]
    C --> D[K-Means Clustering]
    D --> E[Recommendation Engine]
    E --> F[Recommended Anime]
```

---

# 🔄 Recommendation Pipeline

```mermaid
graph TD

User[User enters anime name]
Search[Fuzzy Match]
Vector[TF-IDF Features]
Cluster[K-Means Cluster]
Recommend[Find Similar Anime]
Output[Display Recommendations]

User --> Search
Search --> Vector
Vector --> Cluster
Cluster --> Recommend
Recommend --> Output
```

---

# 🧠 Machine Learning Workflow

```mermaid
flowchart TB

A[Load Dataset]
B[Preprocess Text]
C[TF-IDF]
D[K-Means]
E[Store Clusters]
F[Recommendation Function]

A --> B
B --> C
C --> D
D --> E
E --> F
```

---

# 📂 Dataset

📦 **Top 15,000 Ranked Anime Dataset**

**Modifications**
- Renamed to `anime_2025.csv`
- Removed `japanese_name`

---

# 🚀 Run

```bash
git clone https://github.com/<username>/ani-compass.git

cd ani-compass
```

Open

```
Unsupervised_Anime_Recommendation_System.ipynb
```

Run

```python
get_recommendations("Naruto")

get_recommendations("Bleach")

get_recommendations("Bleech")   # typo handling
```

---

# ⚙️ Tech Stack

```mermaid
mindmap
  root((Ani Compass))
    Python
    Pandas
    NumPy
    Scikit-Learn
      TF-IDF
      K-Means
    NLTK
    Google Colab
```

---

# 📁 Project Structure

```text
ani-compass
│
├── ani-compass/
│   └── project-overview.webp
│
├── dataset/
│   └── anime_2025.csv
│
├── Unsupervised_Anime_Recommendation_System.ipynb
├── README.md
└── LICENSE
```

---

# 🚀 Future Improvements

```mermaid
journey
    title Future Roadmap
    section Phase 1
      Improve Accuracy: 5
      Better Clustering: 5
    section Phase 2
      Streamlit App: 4
      REST API: 4
    section Phase 3
      Hybrid Recommendation: 5
      User Personalization: 5
```

---

# 👨‍💻 Author

**Somapuram Uday**