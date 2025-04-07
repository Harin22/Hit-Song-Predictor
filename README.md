# 🎵 Hit-Song-Predictor

A machine learning project that predicts whether a song will become a hit based on its audio features.

This end-to-end project walks through the full ML pipeline—from loading a real-world Spotify dataset and performing data cleaning and feature engineering to building and evaluating a classification model. The goal is to identify patterns in musical attributes that signal a track's popularity and to **predict hit songs (hit = 1)** based on learned insights.

---

## 🚀 Project Goals

- Load and explore a large Spotify dataset of over 126,000 tracks  
- Clean and preprocess real-world audio features  
- Engineer a target feature based on popularity: **Hit or Not a Hit**  
- Apply feature scaling for ML model readiness  
- Build and evaluate a **Logistic Regression classifier**  
- Understand and explain model performance using accuracy, confusion matrix, and classification report  

---

## 📁 Dataset Summary

The dataset includes audio features and metadata for thousands of Spotify tracks.

**Key features used:**
- `danceability`, `acousticness`, `energy`, `valence`, `speechiness`, `tempo`, `loudness`, `instrumentalness`, etc.
- `explicit`, `key`, `mode`, `year`, `duration_ms`
- Target label `hit`: Created by thresholding Spotify's `popularity` score (hit = 1 if popularity ≥ 20)

---

## 🧰 Technologies Used

- **Python**
- **Pandas**, **NumPy** – for data handling
- **Matplotlib**, **Seaborn** – for EDA and visualization
- **Scikit-learn** – for scaling, modeling, and evaluation

---

## 🧹 Data Preprocessing

- Dropped irrelevant features: `id`, `name`, `artists`, `release_date`
- Converted date columns to datetime format
- Created a new binary label `hit` from the `popularity` column
- Filled missing `tempo` values with the **median**
- Applied `StandardScaler` to normalize numerical features
- Performed `train_test_split` with stratification to preserve class balance

---

## 📊 EDA Insights

- Hit songs tend to have:
  - Higher **energy**, **loudness**, and **danceability**
  - Lower **acousticness** and **instrumentalness**
- Strong positive correlation between `year` and hit likelihood
- `energy` and `loudness` were highly correlated (but both useful)
- Visualized feature distributions and correlation matrix for interpretation

---

## 🧠 Model Built

### ✅ Logistic Regression (Baseline)

- Trained on scaled audio features  
- Tested on unseen data with stratified 80/20 split  
- Achieved **93.3% accuracy**  
- Precision and recall balanced across both classes

**Evaluation Metrics:**

| Metric     | Class 0 (Not Hit) | Class 1 (Hit) |
|------------|-------------------|---------------|
| Precision  | 89%               | 95%           |
| Recall     | 89%               | 95%           |
| F1-score   | 89%               | 95%           |

---

## ✅ Current Project Status

- [x] Data loading, cleaning, and feature engineering  
- [x] Correlation and EDA analysis  
- [x] Feature scaling and train-test split  
- [x] Logistic Regression training and evaluation

---

## 📜 License

This project is licensed under the MIT License.

---

## 🙌 Acknowledgements

- Spotify for dataset inspiration  
- scikit-learn and seaborn for analysis tools  
- Built as a job-ready hands-on machine learning project

---

## 🎯 Finally! 
The model achieved 93.3% accuracy and shows ability to distinguish hit and non-hit songs with balanced precision and recall, without any bias toward class imbalance. 
