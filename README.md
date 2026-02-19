# 🐦 Sentiment Analysis of Tweets

## Project Overview:

This project implements a machine learning–based sentiment analysis system that classifies tweets as Positive or Negative using Natural Language Processing (NLP).The objective is to automatically analyze public opinion expressed on social media and determine the sentiment behind each tweet. This can be useful for brand monitoring, customer feedback analysis, and social media analytics. The system uses TF-IDF vectorization for feature extraction and a Logistic Regression classifier for prediction.

## Features:
1. Text preprocessing and cleaning
2. TF-IDF feature extraction
3. Logistic Regression classification
4. Model saving and loading using Joblib
5. High classification accuracy
6. Easy-to-use prediction pipeline

## Project Workflow:
1. ### Text Preprocessing -

Tweets are cleaned by: Removing URLs, Removing mentions (@username), Removing hashtags (#topic), Converting text to lowercase, Removing special characters and extra spaces

This ensures that only meaningful textual information is used for analysis.

2. ### Feature Engineering -

The cleaned text is transformed into numerical vectors using TF-IDF (Term Frequency–Inverse Document Frequency). This technique captures the importance of words within tweets and improves model performance.

3. ### Model Training

A Logistic Regression classifier is trained on labeled tweet data to learn sentiment patterns.

4. ### Prediction

The trained model predicts sentiment for new tweets. Example: -

"I love this product!"        → Positive
"This service was terrible."  → Negative

## Model Performance:

The model was evaluated on a separate test dataset:

**Accuracy:** 89.4%
**Precision:** 88.7%
**Recall:** 90.1%
**F1 Score:** 89.3%

## Technologies Used:
1. Python
2. scikit-learn
3. Pandas
4. NumPy
5. Joblib
6. Regular Expressions (Regex)

## Dataset:

Dataset link used for training: https://www.kaggle.com/datasets/krishbaisoya/tweets-sentiment-analysis
The dataset contains labeled tweets categorized as positive or negative sentiment.
