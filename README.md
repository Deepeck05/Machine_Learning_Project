Spam Email Classification — Logistic Regression

Author: Deepeck (aka Mr Cool)
Short bio: I enjoy listening to music, drawing, and dancing. This repository contains a compact, end-to-end Spam Email Classification project using TF-IDF features and Logistic Regression as a baseline model.

Overview

This project demonstrates a standard NLP classification pipeline for detecting spam emails:

Data loading and cleaning

Text preprocessing (tokenization, stopwords, optional lemmatization/stemming)

Feature extraction with TfidfVectorizer

Model training using Logistic Regression

Evaluation with classification metrics (precision, recall, F1, support), confusion matrix, and ROC/PR analysis

Use this repository as a baseline for experimentation (try different vectorizers, models, thresholds, or class-imbalance strategies).

Key Features

TF-IDF text vectorization (configurable ngram_range, min_df, max_df)

Logistic Regression baseline with probability thresholding

Standard evaluation: classification report, confusion matrix, accuracy, ROC AUC, precision-recall curve

Simple, reproducible scripts for training and inference

Requirements

Python 3.8+

pandas

numpy

scikit-learn

matplotlib (optional, for plots)

Install dependencies:

python -m pip install pandas numpy scikit-learn matplotlib

Project Structure (suggested)
README.md
data/
  └─ spam.csv                # (expected: columns: text,label)
notebooks/
  └─ exploration.ipynb
src/
  ├─ preprocess.py
  ├─ features.py
  ├─ train.py
  └─ evaluate.py
models/
  └─ logistic_tfidf.pkl
requirements.txt
