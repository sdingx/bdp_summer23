# Yelp Businesses 

![](Pres_first_page.png)

## Overview
This is a project affiliated with the University of Chicago's Applied Data Science Program. The objective was to create two PySpark-based machine learning solutions on Google Cloud Platform (GCP). These solutions are as follows:

- Sentiment Analysis Model: This model was developed to improve restaurant services by extracting insights from unlabeled short reviews (tips). It focuses on analyzing sentiment within these reviews.
- Personalized Recommender System: The second solution is a personalized recommender system, incorporating two distinct algorithms. One algorithm recommends top users for restaurants, while the other suggests top restaurants to users.

## Project Structure
### 1)Data Download and Import 
- Relevant files: Data_KaggleAPI.ipynb, Data_Import.ipynb
- Utilized the Kaggle API to directly download the 5GB Yelp JSON dataset into Google Cloud Platform (GCP) buckets. Additionally, a data sampling step was conducted to facilitate testing and code validation on a smaller dataset before utilizing extensive computational resources.

### 2)Exploratory Data Analysis
- Relevant file: EDA.ipynb
- An in-depth exploratory data analysis was carried out using BigQuery and Spark SQL on the Yelp dataset. This analysis provided valuable insights into various aspects, including business, reviews, users, and tips.

### 3)Sentiment Analysis Model 
- Relevant files: SentimentAnalysis_SampleData.ipynb, SentimentAnalysis_FullData.ipynb
- To develop a sentiment analysis model, multiple vectorization methods and classification algorithms were tested extensively on a sample dataset first. Once the optimal combination was determined, the model was executed on the full dataset.
- The sentiment analysis models using NLP pipelines and classification models to predict sentiment polarity in tip text data based on a trained dataset of 4.72M Yelp reviews. Following thorough model comparisons and hyperparameter tuning, the LinearSVC model delivered an optimal accuracy rate of 0.8978.

### 4)Recommender System
- Relevant files: Rec_Sys.ipynb, Rec_Sys.html
- A Collaborative Filtering recommender system was developed using PySpark ALS. After hyperparameter tuning, the system achieved an impressive Root Mean Square Error (RMSE) of 0.47. Furthermore, an evaluation was conducted to assess the alignment between the category word clouds of the top 10 recommendations and users' preferences based on their past visits. This assessment confirmed positive validation alongside the RMSE assessment.

## Contact Info
This is a project by Yun Xing ([yxing3@uchicago.edu](mailto:yxing3@uchicago.edu)), Xiran Li ([xiranli16@uchicago.edu](mailto:xiranli16@uchicago.edu)), and Sam Ding ([zding1@uchicago.edu](mailto:zding1@uchicago.edu)). 
Feel free to reach out to them if you have any questions about the project.
