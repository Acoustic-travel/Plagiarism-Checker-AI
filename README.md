# Plagiarism-Checker-AI
## Project Description
This project implements a Plagiarism Checker AI using a Statistical Language Model (SLM) approach. It leverages the MIT Plagiarism Detection dataset from Kaggle, containing around 367,000 sentence pairs labeled as plagiarized or non-plagiarized. The pipeline consists of:
**Data Loading & Cleaning**: Read TSV data, drop missing values, lowercase texts.

**Feature Extraction**: Use CountVectorizer (unigrams + bigrams, top 10,000 features) with built-in stop-word removal.

**Model Training**: Train a Multinomial Naive Bayes classifier (an SLM) on the vectorized text.

**Evaluation**: Report training and testing accuracy, precision/recall/F1, and confusion matrix.

 **Serialization**: Save the trained model and vectorizer to disk for later inference.

No user interface is provided—focus is on backend performance and demonstration of ML pipeline.

### Install Dependencies
pip install -r requirements.txt

### Prepare the Dataset
Download the MIT Plagiarism Detection dataset from Kaggle https://www.kaggle.com/datasets/ruvelpereira/mit-plagairism-detection-dataset

## Sample Results

Classification Report:
              precision    recall  f1-score   support

           0       0.66      0.59      0.62     36586
           1       0.63      0.70      0.66     36888

    accuracy                           0.64     73474
   macro avg       0.64      0.64      0.64     73474
weighted avg       0.64      0.64      0.64     73474


Confusion Matrix:
[[21404 15182]
 [11087 25801]]
 
Accuracy: 0.64247216702507

