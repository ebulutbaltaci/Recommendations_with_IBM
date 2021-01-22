# Recommendations with IBM Project


## 1. Project Motivation

The aim of this project is to analyze the interactions that users have with articles on the IBM Watson Studio platform, and make recommendations of new articles they might like to them.

My project <a href="https://github.com/ebulutbaltaci/Recommendations_with_IBM" target="_blank">GitHub</a> repository.


## 2. Instructions

For this project we will analyze the interactions that users have with articles on the IBM Watson Studio platform, and make recommendations to them about new articles we think they will like. Below is an example of what the dashboard could look like displaying articles on the IBM Watson Platform.

In order to determine which articles to show to each user, we will be performing a study of the data available on the IBM Watson Studio platform.


## 3. Overview

The notebook is divided into below parts:


### 3.1. Exploratory Data Analysis

Before making recommendations of any kind, we will need to explore the data you are working with for the project.There are some basic, required questions to be answered about the data we are working with throughout the rest of the notebook.

### 3.2. Rank Based Recommendations

To get started in building recommendations, we will first find the most popular articles simply based on the most interactions. Since there are no ratings for any of the articles, it is easy to assume the articles with the most interactions are the most popular. These are then the articles we might recommend to new users (or anyone depending on what we know about them).

### 3.3. User-User Based Collaborative Filtering

In order to build better recommendations for the users of IBM's platform, we could look at users that are similar in terms of the items they have interacted with. These items could then be recommended to the similar users. This would be a step in the right direction towards more personal recommendations for the users.

### 3.4. Matrix Factorization

Finally, we will complete a machine learning approach to building recommendations. Using the user-item interactions, we will build out a matrix decomposition. Using our decomposition, we will get an idea of how well we can predict new articles an individual might interact with (spoiler alert - it isn't great). We will finally discuss which methods you might use moving forward, and how you might test how well your recommendations are working for engaging users.


## 4. Running

In a terminal or command window, navigate to the top-level project directory ```Recommendations_with_IBM/``` and run one of the following commands:

```ipython notebook Recommendations_with_IBM.ipynb```

or

```jupyter notebook Recommendations_with_IBM.ipynb```

This will open the iPython Notebook software and project file in your browser.


## 5. Conclusion

There were only 20 customer for which we can try and provide recommendation. If we had more data then performance of our recommendation engine could be evaluated more efficiently. We have a highly imbalanced data because of many zeroes in the user-item interaction matrix. I will try content recommendation in future iteractions to tackle the cold start problem.


## 6. Software Requirements

This project uses **Python 3**.


## 7. Libraries Used

I use Python3. Here are the libraries I used in my Jupyter Notebook:

1. pandas
2. numpy
3. matplotlib.pyplot
4. project_tests
5. pickle
6. sklearn.feature_extraction.text
7. sklearn.decomposition
8. re
9. nltk
10. nltk.tokenize 
11. nltk.stem.wordnet
12. nltk.stem.porter
13. nltk.corpus


## 8. Licensing, Authors, Acknowledgements

This project is apart of Udacity's Data Science Nanodegree Program, which provides initial starter code for the project. Additionally, the original datasets are provided in part by IBM.