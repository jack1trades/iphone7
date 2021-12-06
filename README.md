# Sentiment Analysis of iphone7
## Reviews extracted from amazon.com

## Overview
* Web-scraped and Extracted the reviews for iphone 7 from one of the most popular cybershop website - Amazon
* This project was an Internship project associated with "Innodatatics Inc."
* Optimized several ml algorithms to finalize the best model
* Built a client facing API and user interface

## Code and Resources used
* Python version : Python 3.7
* Packages for web-scraping: bs4, bs4.BeatifulSoup requests, pandas
* Packages for developing back-end code : pandas, numpy, matplotlib, seaborn, sklearn, pickle, fastapi, colabcode

## Project Walk-through

### 1. Web scraping
* Amazon was the preferred cyber-platform for web scraping
* Details like review statements, respective ratings, review date and name of the person who reviewed were extracted
* Columns were named as required

### 2. Back-end
* Dataset : Dataset was read using pandas library.
* As the data was scraped, null values has to be dealt with. 
* EDA & FE : Feature Extraction involved - dealing with null values, deleting superfluous variable columns, and removing punctuations, stopwords, followed by lemmatization.
* The Split : The dataset was divided - predictor(X) and target variable(y). Also, train_test_split was implemented.
* Balance check : Imbalance of target values among observations was found. Upsampling technique was implemented.
* Vectorization : The cleaned dataset was TfidfVectorized - to convert the text language into it's numerical counterpart
* Base Models : Base Regression Classifiers, Support Vector Machines, Decision Tree and KNearestClassifier were implemented. Hyperparameter tuning improvised the model.
* Ensemble Models : Random Forest, and Boosting Algorithms - AdaBoostClassifier, GradientBoostingClassifier, XGBClassifier - were also used, to train the model.
* Inference : RandomForestClassifier gave a maximum accuracy for correct prediction of newly given review statements

### 3. Deployment
* Deployment was achieved via flask.
* The model was successfull enough to give an interactive user interface


# #Done_n_Dusted
