# SMS Spam Detection Using TF-IDF and Machine Learning

## Overview
This lab builds an SMS spam classifier using text preprocessing, TF-IDF feature extraction, and two machine-learning models: Multinomial Naïve Bayes and Logistic Regression. The models are evaluated using a train/test split and five-fold stratified cross-validation.

## Workflow
1. Load the `SMSSpamCollection` dataset from a tab-separated file.
2. Convert messages to lowercase.
3. Remove punctuation, digits, and special symbols.
4. Tokenize messages and remove English stopwords.
5. Join the cleaned tokens into text.
6. Convert messages into TF-IDF feature vectors.
7. Split the data into 80% training and 20% testing sets, preserving label proportions.
8. Train and evaluate Multinomial Naïve Bayes and Logistic Regression.
9. Compare five-fold stratified cross-validation accuracy for both models.

## Technologies Used
- Python
- NumPy
- pandas
- NLTK
- scikit-learn

## Dataset
The notebook expects a file named `SMSSpamCollection` in the Google Colab `/content/` directory. The file should be tab-separated and contain two columns:
- `label`: message category (for example, spam or ham)
- `text`: SMS message content

The notebook does not download the dataset automatically, so upload or place the file in the expected location before running it.

## Models and Evaluation
- **Multinomial Naïve Bayes**
- **Logistic Regression** (`max_iter=1000`)

Evaluation methods:
- Accuracy
- Classification report (precision, recall, and F1-score)
- Five-fold stratified cross-validation accuracy, including mean and standard deviation

## How to Run
1. Open `NLP_Lab09.ipynb` in Google Colab or Jupyter Notebook.
2. Ensure `SMSSpamCollection` is available at `/content/SMSSpamCollection` when using Colab.
3. Install missing dependencies if necessary: `numpy`, `pandas`, `nltk`, and `scikit-learn`.
4. Run all cells in order and compare the model results.

## Notes
- The TF-IDF vectorizer is fitted to the full dataset before the train/test split and cross-validation. For a stricter evaluation that avoids data leakage, fit the vectorizer separately within each training fold using a scikit-learn `Pipeline`.
- The cross-validation scores use the already-created TF-IDF matrix, so the same feature-fitting caveat applies.
- Results depend on the dataset and the preprocessing choices.

## Author
Piyush Prakhar
