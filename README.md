# Drug-Sentimental-Case-Study Analysis 

<img src = '/images/drugs.jpg',title='Drug Condition Predictor'>

## Stakeholders: Drug Manufacturers
## Goals: 

1)Assist drug manufacturers in making informed decisions 
2)Performing Root Cause analysis on the drastic drop in drug ratings over the course of 10 years    
3)Predicting patient conditions using multi-class classification(Naive Bayes and SVM)
4)Performing Sentimental analysis to extract subjective information in patient reviews and help build a generalized understanding the effectiveness of the drugs

## Python Packages: pandas, Numpy, sklearn, seaborn, wordcloud 

## Approach :

1)Perform extensive exploratory data analysis which involves trimming white spaces, removing stop words, using Snowball stemmer, tokenizing, and vectorizing data after scraping drug reviews online 

2)Evaluating performance after performing cross-validation and hold out test validation

3)Evaluating vectorizers, length of document frequency, along with use of ngrams on all multi-class classification algorithms    

## Results:

### Minimum Document Frequency of gives highest f1 score 
### Snowball Stemmer works best 
 
Bernoulli Naive Bayes gives the best results for Boolean vectorizer and ngram(1,3) after using cross-validation keeping alpha =0.01

Multinomial  Naive Bayes gives the best results for TF  vectorizer and ngram(1,3) after using lemmatizer keeping alpha =0.01

Linear SVC gives the highest f1 score of 89% after using TF vectorizer with ngram(1,3) for slack varaible C=1 which maintains bias-variance trade-off

## Linear SVC with term frequency input and ngram range of (1,3) givves precision of 86% and recall of 86% beating best performing Bernoulli NB and Multinomial NB by almost 6% and 4% in terms of precision and by 7% and 12% in terms of recall respectively
 
## Insights:

1)Drug ratings have been falling for the past 10 yearsThe prominent conditions in 2009 is Pain while in 2017 it is Birth Control. Thus, we can come to the conclusion that abortion rates are increasing dramatically. 

2)There is a steady fall in drug ratings as drug reviews for birth control pills is mostly negative 



