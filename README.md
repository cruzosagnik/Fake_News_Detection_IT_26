# Fake_News_Detection_IT_26
A Machine Learning pipeline for binary classification of news articles, distinguishing between verified journalistic reporting and sensationalized/unverified content using NLP techniques and Python.

# Fake News Detection System

## 📌 Project Overview
This project focuses on the binary classification of news articles into two categories: **True** (verified reporting) and **Fake** (unverified or sensationalized content). By leveraging Natural Language Processing (NLP), the system identifies linguistic patterns—such as sensationalist headers, emotional weight, and formal agency datelines—to predict the authenticity of a given text.

## 📊 Dataset Specifications
The model is trained on a comprehensive dataset consisting of ~45,000 articles:
*   **True.csv**: Verified news articles, primarily from Reuters, characterized by neutral tone and formal datelines (e.g., "WASHINGTON (Reuters)").
*   **Fake.csv**: Unverified articles often containing high-arousal emotional language, conspiracy-leaning narratives, and social media calls to action.

### Data Structure
The processed dataframe (`df`) uses a simplified schema for optimal training:
*   `title`: The headline of the article.
*   `text`: The full body content.
*   `label`: `1` for True, `0` for Fake.

## 🛠️ Tech Stack
*   **Language:** Python 3.10
*   **Data Analysis:** Pandas, NumPy
*   **Machine Learning:** Scikit-learn (TF-IDF Vectorization, Logistic Regression/Passive Aggressive Classifier)
*   **NLP:** NLTK / Spacy (Tokenization, Stop-word removal)

## 🚀 Key Features
*   **Linguistic Pattern Recognition**: Distinguishes between formal wire-service styles and informal social media styles.
*   **Optimized Pipeline**: Efficient text preprocessing and vectorization.
*   **Real-time Prediction**: A script to input custom news text and receive an immediate classification score.

## 📈 Performance
*   **Class Balance**: Approximately 52% Fake / 48% True.
*   **Evaluation Metrics**: Accuracy, Precision-Recall Curve, and F1-Score.


