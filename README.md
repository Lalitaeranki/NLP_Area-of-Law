
# NLP Approach to identify Area of Law for Indian Law Judgement

## Objective
The objective is to predict and label 100 Indian Law Judgements out of 999 Judgements.

## Data
Data set -The link for the Judgement folder is given below and in folders Fixed Judgement.
https://www.dropbox.com/s/vz5cnytqrz1acol/Fixed%20Judgements.zip?dl=0

The link for mapping files as below and in file Interview_Mapping.csv.
https://www.dropbox.com/s/mxtntuct1ssg5l2/Interview_Mapping.csv?dl=0
Coding is done is Python and different libraries like NLTK,Pandas,scikit-learn are used for the project.

## Data cleansing/manipulation
The Judgment text from the text files is extracted and appended as a column against the Area of Law to form a dataframe in Python.
Since the text files in the Judgement Column is ambiguous and  non standard ,in order to have better accuracy the text is parsed, organised and encoded or vectorized for the machine to understand.
The Natural Language Processing (NLTK platform in Python)is used on  the text from the Judgement Column which are tokenized,stemmed to root word,cleansed by removing stopwords and finally joined .Further the text is vectorized  into vectors based on their frequency of appearance which then using for training and testing.

## Methodology/ML technique used
The training and testing model obtained from the above is then classified using three different classifiers from the  scikit-learn library in Python which are Naive Bayes Classifier,Logistic Regression and Linear SVC (Support Vector Classifier) to fit and predict the model outcome i.e label the 100 unlabeled Judgements.

## Measuring model results/accuracy 
The accuracy for the above three classifiers is calculated 

|Classifier|Accuracy(%)|
|:----------:|:------------:|

Naive Bayes Classifier               52.22
Logistic Regression  Classifier      62.22
Linear SVC                           60.75
The prediction with Logistic Regression Classifier is more fit due to higher accuracy.
