# Word Embeddings with Word2Vec and GloVe

## Overview
This lab explores word embeddings using the NLTK Movie Reviews corpus. It preprocesses review text, trains Word2Vec models using CBOW and Skip-Gram, examines word similarities and analogies, visualizes embeddings with PCA, and compares a trained model with pretrained GloVe vectors.

## Topics Covered
- Lowercasing and tokenization
- Removing punctuation, non-alphabetic tokens, and English stopwords
- Vocabulary construction
- Training Word2Vec with CBOW and Skip-Gram
- Comparing model vocabulary size, embedding dimensions, and training time
- Finding similar words and testing word analogies
- Visualizing 50 word embeddings in two dimensions using PCA
- Comparing cosine similarity from trained Word2Vec and pretrained GloVe embeddings

## Tools and Libraries
- Python
- NLTK
- Gensim
- Matplotlib
- scikit-learn

## Dataset and Embeddings
- **Movie Reviews corpus:** NLTK's `movie_reviews` corpus, used to train Word2Vec models.
- **Pretrained embeddings:** Gensim's `glove-wiki-gigaword-100`, loaded for comparison.

## Main Parameters
- Embedding dimension: `100`
- Context window: `5`
- Minimum word count: `3`
- Word2Vec architectures: CBOW (`sg=0`) and Skip-Gram (`sg=1`)

## How to Run
1. Open `S25MCAG0109_Lab08.ipynb` in Jupyter Notebook or Google Colab.
2. Run the cells in order.
3. Ensure the required packages are installed: `nltk`, `gensim`, `matplotlib`, and `scikit-learn`.
4. Allow NLTK to download the Movie Reviews corpus, tokenizer resources, and English stopwords.
5. Allow Gensim to download the pretrained GloVe vectors when that cell runs.
6. Review the printed model details, word similarities, analogies, and PCA plot.

## Learning Objectives
- Understand how words are represented as dense vectors.
- Compare CBOW and Skip-Gram Word2Vec training.
- Explore semantic similarity and vector analogies.
- Visualize high-dimensional word vectors in two dimensions.
- Compare embeddings trained on a specific corpus with pretrained embeddings.

## Notes and Limitations
- The Movie Reviews corpus is focused on movie-review language, so the trained embeddings reflect that domain.
- Word analogy results depend on whether the required words exist in the trained vocabulary; some queries may fail if a word is missing.
- PCA compresses vectors for visualization and does not preserve all embedding information.
- The pretrained GloVe model is trained on a different, much larger text source, so its similarity scores are not a direct quality comparison with the lab-trained model.

## Author
Piyush Prakhar
