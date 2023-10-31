# NLP - Yelp Reviews Classification

## 📌 Introduction
This project is to classify Yelp Reviews into 1 star or 5 star categories based off the text content in the reviews. The data used in this project is from Yelp Review Data Set from Kaggle. Each observation in this dataset is a review of a particular business by a particular user.

## 📚 Data
- Dataset taken from [Yelp Review Data Set from Kaggle](https://www.kaggle.com/c/yelp-recsys-2013).
- Each observation in this dataset is a review of a particular business by a particular user.
- The "stars" column is the number of stars (1 through 5) assigned by the reviewer to the business. (Higher stars is better.) In other words, it is the rating of the business by the person who wrote the review.
- The "cool" column is the number of "cool" votes this review received from other Yelp users. 
- All reviews start with 0 "cool" votes, and there is no limit to how many "cool" votes a review can receive. In other words, it is a rating of the review itself, not a rating of the business.
- The "useful" and "funny" columns are similar to the "cool" column.

## 💻 Technologies
- [Python](https://www.python.org/): Programming language
- [Pandas](https://pandas.pydata.org/): Data analysis and manipulation tool
- [Numpy](https://numpy.org/): Library for adding support for large, multi-dimensional arrays and matrices
- [Matplotlib](https://matplotlib.org/): Library for creating static, animated, and interactive visualizations
- [Seaborn](https://seaborn.pydata.org/): Data visualization library based on matplotlib
- [Scikit-learn](https://scikit-learn.org/stable/): Machine learning library for the Python programming language
- [Natural Language Processing](https://en.wikipedia.org/wiki/Natural_language_processing): Natural language processing (NLP) is a subfield of linguistics, computer science, and artificial intelligence concerned with the interactions between computers and human language, in particular how to program computers to process and analyze large amounts of natural language data.

## 📜 Project
- Exploratory Data Analysis
- Natural Language Processing
- Model Evaluation

## 🧩 Exploratory Data Analysis
- Importing libraries and dataset
- Exploring the dataset
- Creating a new column called "text length" which is the number of words in the text column
- Exploring the dataset
- Data Visualization

## 🧠 Natural Language Processing
- Importing CountVectorizer and creating a CountVectorizer object
- Using the fit_transform method on the CountVectorizer object and passing in X (the 'text' column). Saving this result by overwriting X
- Importing TfidfTransformer from sklearn
- Importing Pipeline from sklearn.pipeline
- Creating a pipeline with the following steps:CountVectorizer(), TfidfTransformer(),MultinomialNB()
- Using the pipeline to fit the training data
- Predicting off the test set and creating a classification report and confusion matrix using these predictions

## 📈 Model Evaluation
- Importing TfidfVectorizer from sklearn
- Importing TfidfTransformer from sklearn
- Importing MultinomialNB from sklearn.naive_bayes
- Importing Pipeline from sklearn.pipeline
- Creating a pipeline with the following steps:CountVectorizer(), TfidfTransformer(),MultinomialNB()
- Using the pipeline to fit the training data
- Predicting off the test set and creating a classification report and confusion matrix using these predictions

## 🎯 Conclusion
- The model is performing very well with 81% accuracy.