# Quora Duplicate Questions Detection

This project aims to identify whether two given questions from Quora are semantically duplicate or not. Duplicate questions often clutter search results and reduce content quality — detecting them helps improve user experience.

## Dataset
You can download the dataset from: https://www.kaggle.com/c/quora-question-pairs

## Approach
- **Text Preprocessing**: Removed stopwords, punctuation, special characters, and normalized text.
- **Feature Engineering**: Extracted similarity features such as common words, total words, token-based metrics, length-based features, and fuzzy matching scores.
- **Vectorization**: Used **Bag of Words (BOW)** representation via `CountVectorizer` to convert text data into numerical vectors.
- **Model**: Trained a **Random Forest Classifier** on the engineered features combined with BOW vectors.
- **Evaluation**: Assessed model performance using accuracy, precision, recall.

## How to Run
1. Clone the repository.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
