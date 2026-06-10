# 🎵 Intelligent Music Recommender System

> Discover songs that feel just like your favourite track — powered by acoustic feature analysis & cosine similarity

---

## About This Project

### Architecture
A content-based music recommendation engine using Spotify audio features and cosine similarity. The system is trained on a global multi-million-song dataset and computes similarity on-demand — no NxN matrix, making it scalable to 1M+ songs across any genre or language.

---

## How Recommendations Work

1. **Feature Extraction** — Each song becomes a 9-dimensional vector of Spotify audio features
2. **Normalisation** — Min-Max scaling to [0, 1] for fair comparison
3. **Cosine Similarity** — One seed vector vs all N songs via fast matrix multiplication
4. **Filtering** — Language, Genre, and Audio Feature bucket filters
5. **Ranking** — Top-N most similar songs returned with confidence scores

---

## Audio Features

| Feature | Range | What it measures |
|---|---|---|
| Danceability | 0–1 | Rhythmic suitability for dancing |
| Energy | 0–1 | Intensity & perceptual activity |
| Loudness | dB | Average loudness |
| Speechiness | 0–1 | Spoken word presence |
| Acousticness | 0–1 | Acoustic confidence |
| Instrumentalness | 0–1 | No-vocals prediction |
| Liveness | 0–1 | Live audience presence |
| Valence | 0–1 | Musical positiveness (happiness) |
| Tempo | BPM | Beats per minute |

---

## Dataset

The recommender is trained on a combined global dataset drawn from multiple Spotify data sources, covering millions of tracks spanning Pop, Rock, Hip-Hop, Jazz, Electronic, Classical, Folk, Anime, Country, R&B, Indie, and many more genres. Data preparation merges, deduplicates, and standardises all sources into a single optimised CSV.

---

## Tech Stack

`Python` · `Streamlit` · `scikit-learn` · `pandas` · `NumPy` · `Plotly` · `SciPy`

---

## Team

| Name | Roll Number |
|---|---|
| Abhay Pandit | 0002CD231001 |
| Aman Sen | 0002CD231007 |
| Anany Mishra | 0002CD231008 |
| Varun Gupta | 0002CD231075 |

**Under Guidance Of**
- Mr. Madhav Chaturvedi — Assistant Professor
- Mr. Gajendra Kumar Ahirwar — Assistant Professor

**Bachelor of Technology — Computer Science Engineering (Data Science)**
School of Information Technology, R.G.P.V, Bhopal
