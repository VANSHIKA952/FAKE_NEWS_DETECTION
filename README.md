# FAKE_NEWS_DETECTION
PROBLEM STATEMENT:

## FAKE NEWS DETECTION

## INTRODUCTION:

In short, our project includes classifying news as real or fake. For a number of news articles, we used web scraping, which involves scraping news websites. Additionally, it makes use of various machine learning methods and natural language processing techniques to categorise fake news articles using Python's SciKit packages.

## DATASET:
LIAR plus

[Dataset link](https://github.com/VANSHIKA952/FAKE_NEWS_DETECTION/tree/main/Dataset/)

Below are the columns used  in this project:

- column 1:author 

- column 2:statement

- column 3:Label

You will see that newly created dataset has only two classes for classification as compared to six classes.Below is how the values are reduced to true and false.

- False--False

- True--True

- Mostly-true-True

- Half-true--True

- Barely-true--True

- Pants-fire--False

The dataset used for this project were in tsv format named train.tsv , test.tsv , valid.tsv

## File descriptions

### DataPreprocess.py

This file contains all the preprocessing functions needed to process the input data.
First we read the data set and then perform some preprocessing like punctuation removal,tokenisation,stopwords removal,stemming and lemmatization.**We have also used skip grams which is also the novelty in our projec**t. There is also some analysis performed on the data like target variable distribution using wordcloud and data quality check like missing values.Next we performed feature extraction and selection methods using sci-kit learn python libraries.For feature selection we have used methods like bag-of-words and then  term-frequency like tf-idf weighting.


### classifiers.py

In this file we have build different classifiers for predicting the fake news.The extracted features are fed into various classifiers.Here in our project we made use of Naive-bayes,Logisitic regression,Random forest and decision tree classifier from sklearn.Once the model is fitted using extracted features, we predict the values.After prediction,we compare f1 score and check the confusion matrix.The best model is selected for fake news classification.
We have also extracted top features from tf-idf vectorizer to see which words are most important in each of the classes.

