# 🎭 IMDB Sentiment Analyzer

A Machine Learning model to classify IMDB movie reviews as **Positive** or **Negative** using `CountVectorizer`, `TfidfTransformer`, and `LogisticRegressionCV`.

📈 Achieved **~89.63% Test Accuracy**.

---

## 📌 Project Overview
- **Dataset:** IMDB Dataset of 50,000 Movie Reviews ([Kaggle](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews))  
- **Model:** Logistic Regression with cross-validation (on TF-IDF transformed reviews)  
- **Preprocessing:** Stopword removal, tokenization, TF-IDF feature extraction  
- **Output:** Trained model saved as `save_model.sav`  
- **Usage:** Predicts sentiment (positive/negative) of unseen movie reviews  

---

## 🗂 Project Structure
