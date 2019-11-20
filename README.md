## Project Motivation
This project is part of Udacity Data Science Nanodegree Capstone. Starbucks’ is known for its exclusive offers, in this project we are provided with a simulated data that mimics customer behavior on the Starbucks rewards mobile app. Offers are of different types, and not all customers receive same offers, also there might be some customers who do not receive any offer during certain weeks.

## Project Goals
In this project, I will be analyzing starbucks offer and customer transcation data to see what different types of offers are in data, what a successful offer means for each type, and what features in the dataset have most impact on predicting offer's success. I will be using supervised learning techniques to predict offer's success and identifying top features in the dataset with most predictive power

## File Description
- Capstone File.zip: There are three json files in the Capstone Files folder that contain the raw data:
  a) Portfolio - includes information on different starbucks offers
  b) Profile - Customer demographics- any population that received/viewed/completed the offer
  c) Transcript - Customer transaction data
- Starbucks_Capstone_notebook - this is a jupyter notebook, and contains all the analysis regarding the project including data clean up, exploratory analysis, machine learning model implementation, evaluation and results, and overall observations from the analysis.
- Visuals.py - A python support file to run certain codes in the jupyter notebook

## Installation and libraries
This code is in Python and requiures python 3 to run the files. Libraries that were used
- Pandas
- Numpy
- Matplotlib
- Seaborn
- Scikit-learn

## Project Description
My main focus in this project was defining a successful offer, and what features in the dataset have a high impact on offer’s success. In the process I had to clean and process data, drop any outliers, or missing information that didn’t add any value to the analysis. Since I wanted to evaluate if an offer will be successful or not, which is a classification scenario, I used ensemble methods : RandomForest, AdaBoost, and GradientBoostingClassifiers for predictions along with Naives Predictor. I then chose GradientBoostingClassifier as my final model due to it’s high accuracy and f score on test data and shorter training time. Finally I used Feature Importance function to determine the features that have most impact on offer’s success.

## Results

- Overall my observations in this project were as follows:
  1. Among the people who received an offer, there was larger percentage of male population (58%) compared to females (42%).
  2. Offer’s success percent was slightly higher among females (20%) compared to males(18%), although for informational offers male       population responded slightly better than females.
  3. Most of the offers were either BOGO or discount, and few informational
  4. Success percent was slightly higher for BOGO and discount offers (20%) compared to informational (15%) which might be attributable to reward associated with bogo/discount offers
  5. Accuracy score with GradientBoosting classifier on combined dataset (includes all offer types) was 0.8738, and fscore was 0.7021 and scores were way better than naive predictor performance. This shows higher efficiency in using GradientBoosting model
  6. Features that had most impact on offer’s success were — transaction (customer makes a transaction), customer’s membership tenure, age, income, and reward received on completing the offer.

Detailed results of this analysis can be viewed on <a href="https://medium.com/@joshsgm/an-analysis-on-starbucks-offer-data-694929def514">Medium</a>.

## Refernces
Code references were from other Udacity projects
