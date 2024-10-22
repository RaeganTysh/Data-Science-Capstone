# Winning the Space Race - SpaceX Falcon 9 Launch Analysis

## This project analyzes SpaceX Falcon 9 rocket launches by leveraging data visualization and machine learning techniques to predict the likelihood of successful launches. It covers the entire data science lifecycle, from data collection to the deployment of a machine learning model.

### Table of Contents
- [Project Overview](#project-overview)
- [Data Collection](#data-collection)
- [Data Wrangling and Cleaning](#data-wrangling-and-cleaning)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Visualization and Mapping](#data-visualization-and-mapping)
- [Feature Engineering](#feature-engineering)
- [Machine Learning Model Development](#machine-learning-model-development)
- [Model Evaluation](#model-evaluation)
- [Conclusion and Findings](#conclusion-and-findings)

## Project Overview
The goal of this project is to analyze the outcomes of Falcon 9 launches and build a predictive model to determine the success probability of future launches. The analysis uses various data sources to extract insights and create a machine learning model that predicts launch success.

## Data Collection
The data used in this project was gathered from the following sources:
- SpaceX Launch Data: The Falcon 9 launch data was collected using SpaceX's public API and historical launch records. This includes information about the launch date, site, payload mass, orbit type, booster version, and launch outcome.
- Weather Data: Historical weather data was also collected to understand its potential impact on launch success.
- Geospatial Data: Geographical coordinates of the launch sites were used for map visualization.

## Data Wrangling and Cleaning
The collected data went through a series of data cleaning steps, including:
- Handling missing values.
- Converting data types for consistency.
- Removing duplicate records.
- Formatting columns such as date, time, and coordinates.

## Exploratory Data Analysis (EDA)
EDA was performed to uncover patterns and trends in the data. The following analyses were conducted:
- Launch Outcome Analysis: Identifying factors that contribute to launch success or failure.
- Correlation Analysis: Determining the relationship between variables such as payload mass, orbit type, weather conditions, and launch outcomes.
- Temporal Trends: Analyzing the changes in launch success rates over time.

## Data Visualization and Mapping
A Folium map was created to visualize the geographical distribution of launch sites and their outcomes. The map includes:
- Markers: Indicating launch sites with color-coded markers for successful (green) and unsuccessful (red) launches.
- Circles: Displaying the proximity of launch sites to nearby key locations, such as coastlines and highways.
- Zoomed Views: Focused views on individual launch sites like Kennedy Space Center to highlight detailed launch histories.

## Feature Engineering
New features were engineered to enhance the predictive power of the machine learning model:
- Derived Features: Created features such as "Distance to Coast" and "Payload-to-Orbit Ratio."
- Categorical Encoding: Encoded categorical variables like "Orbit Type" and "Booster Version" into numerical formats.
- Scaling and Normalization: Applied scaling techniques to normalize numerical features.

## Machine Learning Model Development
The predictive modeling process involved the following steps:
1. Model Selection: Various models such as Logistic Regression, Decision Trees, Random Forests, and Support Vector Machines (SVM) were tested.
2. Hyperparameter Tuning: Optimized model parameters using techniques like Grid Search and Random Search.
3. Training and Validation: Split the dataset into training and test sets for model training and evaluation.

## Model Evaluation
The model performance was evaluated using metrics like:
- Accuracy: The percentage of correctly predicted outcomes.
- Precision and Recall: To assess the model's ability to correctly identify successful launches.
- Confusion Matrix: Provided a detailed breakdown of true positives, true negatives, false positives, and false negatives.
- ROC Curve and AUC: Measured the model's ability to distinguish between successful and failed launches.

## Conclusion and Findings
The analysis revealed several key insights:
- Geographical Distribution: Launch sites on the East Coast tend to cater to geostationary missions, while West Coast sites focus on polar orbits.
- Significant Factors: Variables such as payload mass, weather conditions, and orbit type have a considerable impact on launch success.
- Model Accuracy: The best-performing model achieved an accuracy of over 85% in predicting launch outcomes.
