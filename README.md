# Sparkify Project

This repository contains the results of the Capstone Sparkify Project from my Data Science Nanodegree. It gives the reviewer access to my code. For further information look at my [medium blog post](https://medium.com/@nicole.a/big-data-analytics-with-spark-83f4fc3147a1).


### Overview
In this project I worked with the data of Sparkify - a fictional music streaming provider. Sparkify collected a lot of data from users and provided them in a huge dataset. In this project we use and analyse this data of the Sparkify users. To be able to analyze this huge amount of data, tools like Spark are necessary. Spark processes data in a distributed way and additionally analyzes data that doesn´t fit into the memory of a local machine. So in this project I have used Spark to analyze the user event based data. I work on a tiny subset (128MB) of the full dataset available (12GB) since the analysis is done on a local machine. The goal is to predict the user churn.

### Project Challenge
The challenge of this project is to understand the features which can indicate the customers churn behavior from a business perspective. By getting an understanding of these features, it is possible to prevent certain users to churn. The first challenge is to find the features which can predict churn behavior, then train a predictive model - using several Machine Learning techniques - on a big amount of data.

### Project Strategy
I will tackle the problem in two steps. First I will explore and clean the data, for example by removing missing or empty values. In this step I will also engineer the features that can be used to predict churn behavior. In the second step I will use different Machine Learning Models to be able to predict customer churn. The metric that I will want to optimize will be the f1-score.

### Project Data
The used data is provided in a JSON format. It won´t be included in the Repository, as it exceeds the volume that can be uploaded to GitHub. The complete dataset can be found here: s3n://udacity-dsnd/sparkify/sparkify_event_data.json.

### Project Files
The Repository contains this README.md and a folder called Applications, which contains:

- Sparkify.ipynb - Jupyter Notebook that contains analysis, exploring and cleaning data, feature engineering, modeling and improvements
- Sparkify.html - html version of the Notebook

### Project Results
I copared the results of three different Machine Learning techniques: Logistic Regression and Gradient Boosted Trees Classifier and the Random Forest Classifier. The f1-scores are as followed:

- Logistic Regression Model: 77,7 %
- Gradient Boosted Trees Classifier: 99,6 %
- Random Forest Classifier: 92,6 %

### Project Improvements
Improvements to the results might occur by applying further approaches such as:

- Including several more features
- Consider more machine learning models
- Use Grid Search for hyperparameter tuning
- Use the full dataset with a bigger amount of data

### Packages
The following software and packages are necessary to run the notebook:
- Python
- Spark
- Pyspark
- Matplotlib
- Seaborn
- numpy
- pandas
