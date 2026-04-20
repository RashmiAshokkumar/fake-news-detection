# fake-news-detection

1. Introduction
The rapid spread of misinformation and fake news on social media and online platforms poses a serious threat to society. Manual fact-checking is too slow and too costly to scale. Machine learning offers an automated approach to classify news articles as real or fake based on their textual content.
This report documents the complete NLP-based machine learning pipeline for fake news detection — from raw text data to a trained and evaluated classifier ready for deployment.

Dataset: Kaggle — ISOT Fake News Dataset (University of Victoria) Fake Articles: 23,481 | Real Articles: 21,417 | Total: 44,898 Features: Article title, text body, subject category, publication date

2. Problem Statement
The objective is to build a binary text classification model that can automatically determine whether a given news article is fake (label = 1) or real (label = 0), using only the article's text content.

Key Challenges:
•	Text data requires NLP preprocessing before it can be fed into ML models
•	Fake news uses deceptive language — subtle patterns require careful feature extraction
•	Vocabulary is large and sparse — TF-IDF handles this but dimensionality is high
•	The model must generalize to unseen articles, not just memorize training examples
