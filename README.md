# disaster_tweets






About
=====
This project is inspired by Halide Bey's PyCon UK 2018 presentation and associated [repo](https://github.com/halidebey/PyCon2018/blob/master/analysis.py). She uses the Social Media Disasters Dataset from Figure-Eight.com, which contains 10K+ tweets containing terms suggesting they may refer to a disaster. The dataset can be found by searching the page for 'Disasters on social media'. 
  
Some of the tweets use figurative language, and therefore, do not refer to actial disasters. For example:
  
  "Rave in the woods was incredible, we burned the place to the ground!"
  
The dataset includes labels indicating which of the tweets refer to actual disasters. Halide uses logistic regression to create a classifier with a baseline accuracy of ~78%. The aim of this project is to examine other Machine Learning models to determine if this accuracy score can be improved. For the sake of consistency, we have preserved Halide's original train/test split. 
  
We are also indebeted to Sabber Ahamed's excellent series on [Medium](https://medium.com/@sabber/classifying-yelp-review-comments-using-lstm-and-word-embeddings-part-1-eb2275e4066b) and corresponding git [repo](https://github.com/msahamed/yelp_comments_classification_nlp) for outlining an approach to LSTM-based sentiment analysis using Keras. Furthermore, we have utilized Alex Sánchez's custom implimentation of NBSVM, outlined in the comments of this Kaggle [kernel](https://www.kaggle.com/jhoward/nb-svm-strong-linear-baseline), in order to test an additional approach against Sklearn's SVM and Multinomial Naive Bayes classifiers.


Dependencies
============
Python 3.6.* 
Pandas  
Numpy  
Sklearn 
Scipy
Keras
NLTK
Plotly
