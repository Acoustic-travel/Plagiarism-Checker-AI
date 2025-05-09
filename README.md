# Plagiarism-Checker-AI
## Project Description
This project implements a Plagiarism Checker AI using a Statistical Language Model (SLM) approach. It leverages the MIT Plagiarism Detection dataset from Kaggle, containing around 367,000 sentence pairs labeled as plagiarized or non-plagiarized. The pipeline consists of:
#### Data Loading & Cleaning:
Read TSV data, drop missing values, lowercase texts.

#### Feature Extraction:
Use CountVectorizer (unigrams + bigrams, top 10,000 features) with built-in stop-word removal.

#### Model Training: 
Train a Multinomial Naive Bayes classifier (an SLM) on the vectorized text.

#### Evaluation: 
Report training and testing accuracy, precision/recall/F1, and confusion matrix.

#### Serialization:
Save the trained model and vectorizer to disk for later inference.
