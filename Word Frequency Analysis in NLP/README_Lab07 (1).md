# Word Frequency Analysis, Stemming and Lemmatization

## Overview
This lab uses the **news category of the Brown Corpus** to explore word frequency analysis and compare stemming with lemmatization using Python and NLTK.

## Tasks Covered
- Download and load the Brown Corpus news category.
- Tokenize the corpus into words.
- Calculate word frequencies using `FreqDist`.
- Display the 20 most frequent words in a bar chart.
- Apply stemming with `PorterStemmer`.
- Apply lemmatization with `WordNetLemmatizer`.
- Compare stemmed and lemmatized frequencies for selected words.

## Tools and Libraries
- Python
- NLTK
- Matplotlib
- WordCloud
- pandas

## Dataset
The notebook uses the **Brown Corpus**, specifically its `news` category, accessed through NLTK.

## How to Run
1. Open `S25MCAG0109_Lab07(1).ipynb` in Jupyter Notebook or Google Colab.
2. Run the cells in order.
3. Allow NLTK to download the required Brown Corpus, tokenizer, WordNet, and Open Multilingual Wordnet resources.
4. Review the token count, frequent-word chart, and stemming/lemmatization comparisons.

## Learning Objectives
- Analyze word frequencies in a text corpus.
- Visualize the most frequent words.
- Understand the difference between stemming and lemmatization.
- Compare how stemming and lemmatization transform words and affect frequency counts.

## Notes
- Stemming reduces words using rule-based transformations and may produce word forms that are not dictionary words.
- Lemmatization aims to return a dictionary base form; results can depend on the input and part-of-speech information.
- In this notebook, `WordNetLemmatizer` is called without specifying a part of speech, so it uses its default noun setting.

## Author
Piyush Prakhar
