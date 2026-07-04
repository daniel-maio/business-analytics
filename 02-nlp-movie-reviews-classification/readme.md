
# IMDB Movie Review Sentiment Classification

Machine Learning pipeline for sentiment classification (positive/negative) using IMDB data and Naive Bayes models (Gaussian, Multinomial, and Bernoulli).

## Features
- NLP Text Cleaning: HTML tag stripping (Regex), special character removal, lowercasing, stopword removal, and word stemming via NLTK (`SnowballStemmer`).
- Feature Extraction: Text vectorization using `CountVectorizer`.
- Machine Learning: Performance comparison across Gaussian, Multinomial, and Bernoulli Naive Bayes classifiers.