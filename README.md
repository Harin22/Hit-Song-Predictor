# 🎵 Hit-Song-Predictor

A machine learning project that predicts whether a song will become a hit based on its audio features.

This end-to-end project walks through the full ML pipeline—from loading a real-world Spotify dataset and performing data cleaning and feature engineering to building and evaluating classification models. The goal is to identify patterns in musical attributes that signal a track's popularity and to **predict hit songs** with confidence.

---

## 🚀 Project Goals

- 🔍 Explore and understand the Spotify song dataset  
- 🧼 Clean and preprocess data for modeling  
- 📊 Perform exploratory data analysis (EDA)  
- 🏷️ Define a classification target variable: **Hit** or **Not a Hit**  
- 🤖 Build and evaluate machine learning models  
- 💡 Learn practical, hands-on ML skills by doing  

---

## 📁 Dataset Summary

The dataset consists of over **126,000 songs** with audio features extracted from Spotify.

**Key features include:**
- `danceability`, `acousticness`, `energy`, `valence`, `liveness`, `tempo`, `speechiness`, etc.  
- `duration_ms`: Length of the track in milliseconds  
- `year`, `release_date`: Date/time features  
- `popularity`: A numeric score (0–100) based on Spotify's internal metrics  
- `explicit`: Whether the song contains explicit lyrics (0 or 1)  

---

## 🧰 Technologies Used

- Python 🐍  
- Pandas & NumPy for data manipulation  
- Matplotlib for EDA and visualization  
- Scikit-learn for model building and evaluation  

---

## 🧹 Data Preprocessing

- Removed non-numeric or irrelevant columns (`id`, `name`, `artists`)  
- Converted `release_date` to datetime  
- Filled missing value in `tempo` using the **median**  
- Removed duplicates and verified no critical nulls  
- Scaled features using `StandardScaler`  

---

## 📊 EDA (Exploratory Data Analysis)

- Visualized distribution of song popularity  
- Compared distributions across audio features  
- Analyzed correlation among features  
- Detected outliers and skewness where applicable  

---

## 🧠 Models Built

Initial model: **Logistic Regression** (Baseline)
---

## 🏁 Project Status

✅ Completed:
- Data understanding and cleaning  
- Popularity-based binary classification setup  
- EDA and feature selection  
- Logistic Regression model training and evaluation  

🔜 Next Steps:
- Model comparison (Random Forest, SVM, XGBoost)  
- Hyperparameter tuning (GridSearchCV)  
- Feature importance visualization  
- Deployment (Optional)  

---
## 📜 License

This project is licensed under the MIT License.

---

## 🙌 Acknowledgements

- Spotify for dataset availability  
- Scikit-learn & Matplotlib for ML tools  
- Mentorship and self-learning inspired by practical applications  

---
