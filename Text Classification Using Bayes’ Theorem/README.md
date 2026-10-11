# Sentiment Analysis Using Naïve Bayes

## Overview
This code implements a simple Naïve Bayes classifier to classify text as positive or negative sentiment. It tokenizes the provided text data, estimates class prior and word likelihood probabilities, predicts sentiment for test sentences, and evaluates the predictions.

## Tasks Covered
- Tokenize text using whitespace splitting without removing stopwords.
- Calculate prior probabilities for positive and negative classes.
- Calculate word likelihoods using Laplace smoothing.
- Predict sentiment using log probabilities.
- Calculate precision, recall, accuracy, and F1-score manually.
- Calculate the same evaluation metrics using `scikit-learn`.
- Compare manual and package-based metric results.

## Tools and Libraries
- Python
- pandas
- NumPy
- scikit-learn

## Dataset Files
The notebook expects these CSV files in the working directory:
- `train_100_wl.csv` — training data with labels.
- `test_20_wol.csv` — test text without labels.
- `test_20_wl.csv` — test data with labels for evaluation.

## How to Run
1. Place the three CSV files listed above in the same working directory as the notebook.
2. Open `code.ipynb` in Jupyter Notebook or Google Colab.
3. Install any missing dependencies: `pandas`, `numpy`, and `scikit-learn`.
4. Run the notebook cells in order.
5. Review the predicted sentiments and evaluation metrics.

## Learning Objectives
- Understand the basic workflow of a Naïve Bayes text classifier.
- Distinguish class priors from word likelihoods.
- Use log probabilities to compare sentiment classes.
- Evaluate a binary classifier using common classification metrics.
- Verify manual metric calculations against library implementations.

## Notes
- The model uses a bag-of-words approach and ignores word order.
- Laplace smoothing is used for word likelihood estimates.
- Words not found in the training vocabulary are ignored during prediction.
- Manual and scikit-learn metrics should match when calculated on the same labels and predictions with the same positive-class convention.

## Author
Piyush Prakhar
