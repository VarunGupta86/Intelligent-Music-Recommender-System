# INTELLIGENT MUSIC RECOMMENDATION USING MACHINE LEARNING AND ACOUSTIC FEATURE ANALYSIS
🎵 About This Project
Architecture
A content-based music recommendation engine using Spotify audio features and cosine similarity. The system is trained on a global multi-million-song dataset and computes similarity on-demand — no NxN matrix, making it scalable to 1M+ songs across any genre or language.

How Recommendations Work
Feature Extraction — Each song becomes a 9-dimensional vector of Spotify audio features
Normalisation — Min-Max scaling to [0, 1] for fair comparison
Cosine Similarity — One seed vector vs all N songs via fast matrix multiplication
Filtering — Language, Genre, and Audio Feature bucket filters
Ranking — Top-N most similar songs returned with confidence scores
Audio Features
Feature	Range	What it measures
Danceability	0–1	Rhythmic suitability for dancing
Energy	0–1	Intensity & perceptual activity
Loudness	dB	Average loudness
Speechiness	0–1	Spoken word presence
Acousticness	0–1	Acoustic confidence
Instrumentalness	0–1	No-vocals prediction
Liveness	0–1	Live audience presence
Valence	0–1	Musical positiveness (happiness)
Tempo	BPM	Beats per minute
Dataset
The recommender is trained on a combined global dataset drawn from multiple Spotify data sources, covering millions of tracks spanning Pop, Rock, Hip-Hop, Jazz, Electronic, Classical, Folk, Anime, Country, R&B, Indie, and many more genres. Data preparation merges, deduplicates, and standardises all sources into a single optimised CSV.

Tech Stack
Python · Streamlit · scikit-learn · pandas · NumPy · Plotly
