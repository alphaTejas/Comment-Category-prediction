# Comment Category Prediction

## Overview

This project focuses on building a machine learning pipeline to classify user comments into multiple categories using both textual and structured data. The approach combines Natural Language Processing techniques with traditional machine learning models to improve prediction performance.

## Dataset

The dataset consists of comment text along with additional features such as upvotes, downvotes, emoticon counts, and metadata. The target variable represents the category assigned to each comment.

## Approach

### Data Preprocessing

* Handling missing and inconsistent values
* Encoding categorical variables
* Feature scaling for numerical columns
* Extraction of temporal features from date

### Feature Engineering

* TF-IDF vectorization of comment text (unigrams and bigrams)
* Combination of text features with tabular features
* Creation of derived features where necessary

### Handling Class Imbalance

* Use of class weights in models
* Evaluation using weighted F1-score

### Model Building

The following models were implemented and compared:

* Logistic Regression
* SGD Classifier
* Random Forest
* Gradient Boosting
* XGBoost
* LightGBM

### Hyperparameter Tuning

* Grid Search with cross-validation
* Stage-wise tuning for efficiency

## Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-score (weighted)

## Key Observations

* Text features contribute significantly to prediction performance
* The dataset is highly imbalanced, making F1-score a more reliable metric than accuracy
* Several features exhibit strong skewness and require careful handling

## Project Workflow

1. Data Cleaning
2. Feature Engineering
3. Text Vectorization
4. Feature Combination
5. Model Training
6. Hyperparameter Tuning
7. Evaluation

## Technologies Used

* Python
* Scikit-learn
* Pandas
* NumPy
* XGBoost
* LightGBM
* Matplotlib
* Seaborn

## Future Work

* Incorporating deep learning models such as LSTM or Transformers
* Using pretrained embeddings like BERT
* Advanced feature selection techniques

## Author

Tejas Kumar
