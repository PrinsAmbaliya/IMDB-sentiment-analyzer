# IMDB Sentiment Analyzer

A Machine Learning model to classify IMDB movie reviews as **Positive** or **Negative** using `CountVectorizer`, `TfidfTransformer`, and `LogisticRegressionCV`.

Achieved **~89.63% Test Accuracy**.

---

## Project Overview
- **Dataset:** IMDB Dataset of 50,000 Movie Reviews ([Kaggle](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews))  
- **Model:** Logistic Regression with cross-validation (on TF-IDF transformed reviews)  
- **Preprocessing:** Stopword removal, tokenization, TF-IDF feature extraction  
- **Output:** Trained model saved as `save_model.sav`  
- **Usage:** Predicts sentiment (positive/negative) of unseen movie reviews  

---

## Project Structure
```
├── Sentiment Analysis.ipynb # Jupyter notebook (training + evaluation)
├── save_model.sav # Trained logistic regression model (generated after training)
├── requirements.txt # Python dependencies
├── README.md # Project documentation
├── .gitignore # Ignored files (dataset, checkpoints, cache, etc.)
└── IMDB Dataset.csv # Dataset (download separately, not included in repo)
```

---

## How It Works
1. Load dataset of IMDB reviews (positive/negative).  
2. Preprocess text (stopword removal + TF-IDF transformation).  
3. Train Logistic Regression model with cross-validation.  
4. Save trained model as `.sav` file for later predictions.  
5. Achieve ~89.63% accuracy on test data.  

---

## Installation & Setup
1.  **Clone the Repository**:
    ```bash:
      git clone https://github.com/your-username/imdb-sentiment-analyzer.git
      cd imdb-sentiment-analyzer

2.  **Create a Virtual Environment & Activate It**:
    ```bash
      python -m venv venv
      source venv/bin/activate    # Linux/Mac
      venv\Scripts\activate       # Windows

3.  **install Dependencies**:
    ```bash:
        pip install -r requirements.txt

4.  **Download NLTK stopwords (first-time only)**:
    ```bash:
    python -c "import nltk; nltk.download('stopwords')"

---

## Model Training

- Vectorization: CountVectorizer + TF-IDF Transformer
- Classifier: Logistic Regression with cross-validation
- Evaluation Metric: Accuracy (~89.63%)
- Persistence: Model saved via pickle as save_model.sav

---

## Future Improvements

Explore Deep Learning models (RNN, LSTM, BERT) for better accuracy
Add real-time API with Flask/FastAPI for predictions
Build Streamlit UI for interactive use
Extend to multi-class sentiment (e.g., very positive, neutral, very negative)

---
Author

Prince Ambaliya

GitHub: PrinsAmbaliya

LinkedIn: https://www.linkedin.com/in/prins-ambaliya-bb7546367
