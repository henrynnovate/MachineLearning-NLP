# Text Classification with Multinomial Naive Bayes and Feature Engineering

This Python script performs text classification on a dataset using Multinomial Naive Bayes and various feature engineering techniques. The code uses the scikit-learn library for machine learning tasks, NLTK for natural language processing, and Matplotlib for visualizations.

## Dataset
The code assumes a CSV file named 'bbc_text_cls.csv' containing text data and corresponding labels. The dataset is loaded into a Pandas DataFrame for further processing.

## Data Exploration
A histogram of the class labels is generated using Seaborn to provide an overview of the dataset's distribution.

## Preprocessing and Splitting
The text data is split into training and testing sets using the `train_test_split` function from scikit-learn.

## Feature Engineering
The main class, `Models`, defines various feature engineering methods:

1. **Multinomial Naive Bayes (MNB):** Utilizes the Count Vectorizer to convert text data into numerical features. Training and testing scores, along with the vocabulary size, are printed.

2. **Stopwords Removal (STW):** Removes common English stopwords using the Count Vectorizer. Training and testing scores, along with the vocabulary size, are printed.

3. **Simple Tokenizer (SIM):** Splits text into words using a simple tokenizer. Training and testing scores, along with the vocabulary size, are printed.

4. **Stemming (STEM):** Applies stemming using the Porter Stemmer through the Count Vectorizer. Training and testing scores, along with the vocabulary size, are printed.

5. **Lemmatization (LEM):** Performs lemmatization using WordNet lemmatizer and POS tagging. Training and testing scores, along with the vocabulary size, are printed.

## Visualization
The `run` function executes the feature engineering methods, and a Pandas DataFrame is created to store the performance metrics (training score, testing score, and vocabulary size) for each method. Line charts are generated to visualize the training and testing scores across different feature engineering techniques.

## Usage
1. Ensure the 'bbc_text_cls.csv' file is available with the required columns ('text' and 'labels').
2. Run the script, and the results will be printed along with visualizations.
