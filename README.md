# Assignment 17: Text Cleaning, Preprocessing and NLP Pipeline

## Overview
This project implements a complete Natural Language Processing (NLP) preprocessing pipeline starting from raw textual data and transforming it into model-ready clean text.


## Dataset

**Dataset Name:** SMS Spam Collection Dataset  
**Source:** https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset  

The dataset contains real SMS messages labeled as spam or ham. It was selected because it includes real-world textual challenges such as:
- Mixed casing
- Punctuation and numbers
- URLs and email patterns
- Informal language and slang
- Extra spaces and noisy text



## Objectives

- Understand raw text characteristics and common issues
- Perform basic text cleaning
- Apply advanced noise removal techniques
- Handle stopwords and informal text patterns
- Perform tokenization
- Compare stemming and lemmatization
- Build a reusable NLP preprocessing pipeline


## Technologies Used

- Python
- Pandas
- NLTK
- spaCy
- Regular Expressions (re)

No machine learning models or vectorization techniques were used, as per assignment requirements.



## NLP Pipeline Steps

### Part 1: NLP Pipeline and Basic Cleaning
- Dataset loading and inspection
- Text length analysis
- Lowercasing
- Removal of punctuation
- Removal of numbers
- Removal of extra whitespaces

### Part 2: Advanced Text Cleaning
- URL removal
- Email removal
- HTML tag removal
- Special character cleaning
- Stopword removal
- Handling repeated characters and slang

### Part 3: Basic NLP Preprocessing
- Word tokenization
- Sentence tokenization
- Stemming using Porter Stemmer
- Lemmatization using WordNet and spaCy

### Final Pipeline
A unified preprocessing function was created to perform:
1. Lowercasing
2. Noise removal
3. Stopword removal
4. Tokenization
5. Lemmatization

The processed output is stored as `final_clean_text`.



## Observations

- Basic cleaning improves formatting consistency but does not remove contextual noise.
- Advanced cleaning significantly improves text quality by removing irrelevant patterns.
- Lemmatization preserves semantic meaning better than stemming.
- Proper preprocessing is essential for improving downstream NLP model performance.


## How to Run

1. Install required libraries:
pip install pandas nltk spacy emoji
python -m nltk.downloader punkt stopwords wordnet
python -m spacy download en_core_web_sm

2. Place `spam.csv` in the project folder.

3. Open and run all cells in:
   NLP_Assignment.ipynb



