# News Category Classification

In this project I used REST API to retrieve the news categories and their descriptions from the News API service,
store data into pandas data frame, and perform some text preprocessing on descriptions to convert them to tokens and store them in the database.

## Algorithms used in this project

- Random Forest Classification model
- Decision Tree Classification model
- MultinomialNB Classification model
- K-Neighbors Classification model

## Steps in building this project

### Data retrieveing from the newsAPI client

- Import the NewsAPIClient from the newsapi client library
- Make a request to the newsapi server to retrieve the data
- response of newsapi server is in JSON format
- insert the JSON data into the pandas dataframe

### Steps in Text Preprocessing

- Create word tokens from Description column
- Remove Punctuation
- Remove Stopwords

### Steps in Storing data into MySQL database

- Create connection to the MySQL database
- Create SQL table with category name and description column
- Insert data from pandas dataframe into table

### Building Machine Learning models

- Import machine learning algorithms from Scikit-learn library
- convert the text token into the word vectors
- split the data-set into traning and testing sets
- build the machine learning models
- evaluate each model on testing set
- choose the best model based on performance

## Difficulties in this project

- to gether the data from API
- after gathering the JSON data converting it into pandas dataframe
- performing the text preprocessing
- storing the data preprocessed into sql table
- retreving the sql table data into dataframe to build models
- evaluting the ML models
