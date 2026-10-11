# Email Spam Classification with Naïve Bayes

## Overview
This code explores email spam detection using Bayes' theorem and Naïve Bayes classification. It begins with a small, manually labeled set of example emails and compares a basic probability-based approach with scikit-learn's `MultinomialNB` classifier.

## Topics Covered
- Bayes' theorem basics
- Tokenizing email text
- Estimating word probabilities for spam and ham
- Text preprocessing with lowercase conversion, regular expressions, and stopword removal
- Extracting word-count features
- Training a `MultinomialNB` model
- Evaluating predictions with accuracy and a classification report

## Tools and Libraries
- Python
- NLTK
- scikit-learn
- `re`
- `collections.Counter`

## Dataset
The notebook uses a small, manually defined list of sample emails labeled **Spam** or **Ham** (non-spam). It is a demonstration dataset, not a large benchmark dataset.

## How to Run
1. Open `code.ipynb` in Jupyter Notebook or Google Colab.
2. Run the cells in order.
3. If prompted, allow NLTK to download the English stopword list.
4. Review the word probabilities, extracted features, classifier evaluation, and prediction for the sample email.

## Learning Objectives
- Understand how Bayes' theorem can be applied to text classification.
- Prepare email text for feature extraction.
- Represent text using word counts.
- Train and evaluate a basic Naïve Bayes spam classifier.

## Limitations
- The dataset contains only a few example emails, so the reported performance is not a reliable measure of real-world spam detection.
- The scikit-learn model is evaluated on the same examples used for training; a separate test set would be needed for a meaningful estimate of generalization.
- The simple tokenization and word-count approach may not capture context or more complex language patterns.

## Author
Piyush Prakhar
