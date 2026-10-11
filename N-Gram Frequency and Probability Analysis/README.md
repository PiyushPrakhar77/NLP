# N-Gram Language Modeling

## Overview
This project explores n-gram language modeling using the **Brown Corpus (news category)** with Python and NLTK. It processes the text into tokens, creates unigram, bigram, and trigram sequences, and calculates simple conditional probabilities.

## Topics Covered
- Text normalization using lowercase conversion and regular expressions
- Unigram, bigram, and trigram generation
- Counting n-gram frequencies
- Finding the 20 most frequent bigrams and trigrams
- Calculating bigram and trigram conditional probabilities
- Estimating sentence probabilities using bigram and trigram models

## Tools and Libraries
- Python
- NLTK
- `re` — regular expressions
- `collections.Counter`

## Dataset
The notebook uses the **Brown Corpus**, specifically its `news` category, downloaded through NLTK.

## How to Run
1. Open `code.ipynb` in Jupyter Notebook or Google Colab.
2. Run the cells in order.
3. Ensure the environment has NLTK installed.
4. The notebook downloads the Brown Corpus using `nltk.download('brown')`.
5. Review the token counts, most frequent n-grams, and probability outputs.

## Learning Objectives
- Understand how n-grams represent sequences of words.
- Analyze frequent word combinations in a text corpus.
- Calculate conditional probabilities from observed counts.
- Estimate sentence probabilities using simple bigram and trigram models.

## Notes and Limitations
- The text is converted to lowercase and characters other than English letters are removed.
- The probability calculations use maximum-likelihood frequency estimates without smoothing.
- Unseen n-grams can receive probability zero, which can make a sentence probability zero.
- Sentence probability is computed by multiplying conditional probabilities; the implementation does not include start/end-of-sentence markers.

## Author
Piyush Prakhar
