
# Tweet Similarity Analysis with Transformer Embeddings

This project analyzes the similarity between tweets using Word2Vec embeddings and standard evaluation metrics.

## Project Structure

- [`code.py`](Tweet-Similarity-Analysis-with-Transformer-Embeddings-main/code.py): Main script for preprocessing, pair generation, embedding calculation, and similarity evaluation.
- `train-modifier.xlsx`: Training data containing tweets and users.
- `testmodifier.xlsx`: Test data.


## Requirements

- Python 3.x
- The following libraries:
  - pandas
  - numpy
  - nltk
  - scikit-learn
  - gensim
  - openpyxl

Install them with:

```sh
pip install pandas numpy nltk scikit-learn gensim openpyxl
```

## Usage

1. Place your data files (`train-modifier.xlsx` and `testmodifier.xlsx`) in the project folder.
2. Adjust the file paths in [`code.py`](Tweet-Similarity-Analysis-with-Transformer-Embeddings-main/code.py) if necessary.
3. Run the main script:

```sh
python code.py
```

The script will display precision, recall, and F1 metrics for both training and test data.

## Main Features

- Preprocessing of tweets (lowercasing, punctuation removal, stopwords, lemmatization)
- Generation of same-user and different-user tweet pairs
- Word2Vec embedding calculation for each tweet
- Similarity calculation using Manhattan distance
- Evaluation with precision, recall, and F1-score

## Notes

- The Word2Vec model used is `word2vec-google-news-300` downloaded via Gensim.
- File paths are currently set for Google Colab. Adjust them for your local environment if needed.

## Author

This project was developed for tweet similarity analysis using
