# Social Media Text Cleaning and Normalization Using Regular Expressions

## Overview
This project demonstrates how Python's built-in `re` module can be used to clean and normalize noisy, informal text. The sample paragraphs contain repeated letters, emojis, unusual punctuation, URLs, contractions, slang, and common misspellings.

## Objectives
- Convert text to lowercase.
- Expand selected contractions and informal abbreviations.
- Remove URLs and unsupported special characters.
- Reduce repeated letters and repeated punctuation.
- Replace selected misspellings and informal words using a mapping.
- Normalize extra whitespace.
- Save the cleaned paragraphs to an output text file.

## Technologies Used
- Python
- `re` — Python's built-in regular expression module

## Files
- `code.ipynb` — Jupyter Notebook containing the text-cleaning code.
- `code_Output.txt` — Output showing the cleaned paragraphs.
- `README.md` — Project description and instructions.

## How It Works
The notebook defines two dictionaries:
- `contractions`: maps selected contractions and abbreviations to expanded forms.
- `typo_map`: maps selected informal words and misspellings to standardized forms.

The `clean_text()` function then applies a sequence of transformations:
1. Handles lists of text recursively.
2. Converts text to lowercase.
3. Replaces selected contractions and abbreviations.
4. Removes URLs.
5. Removes characters outside the allowed letters, numbers, whitespace, and basic punctuation.
6. Reduces sequences of three or more repeated characters.
7. Reduces repeated punctuation.
8. Applies the selected typo replacements.
9. Collapses multiple spaces and trims leading or trailing whitespace.

The notebook applies this function to five sample paragraphs and writes the results to `output.txt`.

## How to Run
1. Open the notebook in Jupyter Notebook or Google Colab.
2. Run the code cells in order.
3. Review the printed cleaned text.
4. The notebook writes the cleaned paragraphs to `output.txt` in the current working directory.

## Limitations
- The replacements are rule-based and only cover patterns explicitly listed in the dictionaries.
- Some slang, misspellings, and contractions may remain unchanged.
- Removing emojis and special characters can remove meaning or tone.
- The cleaning rules do not guarantee grammatically correct or semantically equivalent text.

## Author
Piyush Prakhar
