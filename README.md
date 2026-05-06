# AI-Based Sentiment and Trend Analysis System

## Project Overview

This project uses Natural Language Processing (NLP) and machine learning to analyze sentiment in Twitter and Reddit discussions.

The goal is to classify social media text into three sentiment categories:

- Negative
- Neutral
- Positive

The project includes data preprocessing, exploratory data analysis, TF-IDF feature extraction, model training, model comparison, and final evaluation.

## Dataset

The dataset contains social media text from Twitter and Reddit.

Main columns used:

- `final_text` — cleaned text used as input for the model
- `category` — sentiment label used as the target variable

Label meaning:

- `-1` = Negative
- `0` = Neutral
- `1` = Positive

## Project Workflow

1. Load and inspect the dataset
2. Clean and preprocess text data
3. Perform exploratory data analysis
4. Convert text into numerical features using TF-IDF
5. Train multiple machine learning models
6. Compare model performance
7. Select the best model
8. Evaluate the final model

## Models Used

- Logistic Regression
- Naive Bayes
- Linear SVM

## Best Model

The best-performing model was:

**Linear SVM**

## Final Results

| Metric | Score |
|---|---:|
| Accuracy | 0.858654 |
| Precision | 0.858656 |
| Recall | 0.858654 |
| F1-score | 0.857025 |

## Technologies Used

- Python
- Google Colab / Jupyter Notebook
- pandas
- NumPy
- scikit-learn
- NLTK
- matplotlib
- seaborn
- TF-IDF Vectorization
- Linear SVM

## Repository Structure

```text
AI-Based-Sentiment-and-Trend-Analysis-System/
│
├── data/
│   └── eda_social_media_sentiment_dataset.csv
│
├── models/
│   ├── best_sentiment_model.pkl
│   └── tfidf_vectorizer.pkl
│
├── notebook/
│   └── NLP_Social_Media_Sentiment_Analysis.ipynb
│
├── results/
│   ├── final_evaluation_metrics.csv
│   └── model_comparison_results.csv
│
├── README.md
└── requirements.txt
