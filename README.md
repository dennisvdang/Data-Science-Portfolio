![Banner Image](images/banner.webp)

# Data Science Portfolio

This repository is a curated collection of my work and solutions to various case studies projects.

For more of my project work or independent capstones, please visit the pinned repositories on my [Github](https://github.com/dennisvdang) or visit my website: [https://www.dennisvdang.com](https://dennisvdang.com).

## Table of Contents

- **Case Studies**
  - [Customer Segmentation (Clustering Case Study)](#customer-segmentation-clustering-case-study)
  - [Customer Purchasing Prediction (Decision Tree Case Study)](#customer-purchasing-prediction-decision-tree-case-study)
  - [COVID-19 Prediction (Random Forest Case Study)](#covid-19-prediction-random-forest-case-study)
  - [Diabetes Prediction (Grid Search KNN Case Study)](#diabetes-prediction-grid-search-knn-case-study)
  - [London Housing Price Forecasting (Time Series Analysis/EDA Case Study)](#london-housing-price-forecasting-time-series-analysiseda-case-study)
  - [Wine Quality Prediction (Linear Regression Case Study)](#wine-quality-prediction-linear-regression-case-study)
  - [Heart Disease Prediction (Logistic Regression Case Study)](#heart-disease-prediction-logistic-regression-case-study)
  - [Passenger Survival Prediction (Gradient Boosting Case Study)](#passenger-survival-prediction-gradient-boosting-case-study)
  - [Flight Delay Prediction (Bayesian Optimization Case Study)](#flight-delay-prediction-bayesian-optimization-case-study)
  - [Sales Forecasting (Time Series Forecasting with ARIMA Case Study)](#sales-forecasting-time-series-forecasting-with-arima-case-study)

- **Statistical Foundations**
  - [Cosine Similarity](#cosine-similarity)
  - [Euclidean and Manhattan Distance](#euclidean-and-manhattan-distance)
  - [Frequentist Inference](#frequentist-inference)
- **Mini Projects**
  - [API Mini Project](#api-mini-project)
  - [SQL Mini Project](#sql-mini-project)
- **Guided Capstone**
  - [Guided Capstone](#guided-capstone)

# Case Studies

*Below are summaries of case studies that cover a wide range of topics and demonstrate the application of various data science techniques and algorithms.*

## Customer Segmentation (Clustering Case Study)

**Objective**

- Segment customers based on their purchasing behavior and response to marketing campaign offers, and provide insights into the characteristics of each customer segment to enable targeted marketing strategies

**Methodology**

- Cleaned and transformed data to create a matrix of customer responses to different offers
- Applied k-means clustering and determined the optimal number of clusters using the Elbow, Silhouette, and Gap statistic methods
- Visualized the customer segments in a 2D space using Principal Component Analysis (PCA)
- Analyzed the distribution of key features across the identified clusters and revealed the characteristics of each customer segment
- Libraries: `Pandas`, `Scikit-learn`, `Matplotlib`, `Seaborn`

**Key Takeaways**

- Identified distinct customer segments with varying offer preferences and purchasing behaviors
- Demonstrated the effectiveness of k-means clustering for customer segmentation
- Highlighted the importance of feature selection and dimensionality reduction for effective clustering and visualization

![Customer_Segmentation](images/customer_segmentation.png)

[Link to Customer Segmentation Case Study notebook](https://github.com/dennisvdang/Springboard-Portfolio/blob/main/Case%20Studies/Customer%20Segmentation%20(Clustering%20Case%20Study)/Clustering%20Case%20Study%20-%20Customer%20Segmentation%20with%20K-Means%20-%20Tier%203.ipynb)

## Customer Purchasing Prediction (Decision Tree Case Study)

**Objective**

- Build a predictive model to estimate the likelihood of RR Diner Coffee's loyal customers purchasing the Hidden Farm coffee

**Methodology**

- Analyzed customer data such as age, gender, salary, online purchases, distance from the flagship store, and spending habits to understand key drivers of customer purchasing behavior
- Implemented four decision tree models with varying parameters to understand the impact of different parameters on model performance:
    1. Default Decision Tree Model
    2. Decision Tree with Max Depth = 3
    3. Decision Tree with Min Samples Split = 10
    4. Decision Tree with Min Samples Leaf = 5
- Evaluated model performance using accuracy, balanced accuracy, precision, and recall metrics
- Compared the performance of a single decision tree model to a Random Forest ensemble model
- Libraries: `Pandas`, `Scikit-learn`, `Matplotlib`

**Key Takeaways**

- Identified key factors influencing customer purchasing decisions
- Demonstrated the effectiveness of decision trees for predictive modeling
- Highlighted the importance of model simplicity and interpretability for specific datasets

![Decision_Tree](images/decision_tree.png)

[Link to Customer Purchasing Prediction Case Study notebook](https://github.com/dennisvdang/Springboard-Portfolio/blob/main/Case%20Studies/Customer%20Purchasing%20Prediction%20(Decision%20Tree%20Case%20Study)/Springboard%20Decision%20Tree%20Specialty%20Coffee%20Case%20Study%20-%20Tier%203.ipynb)

## COVID-19 Prediction (Random Forest Case Study)

**Objective**

- Predict the severity of COVID-19 cases using patient characteristics and symptoms

**Methodology**

- Preprocessed and explored the dataset to understand feature-target relationships
- Built and evaluated random forest models with different hyperparameters and feature subsets
- Interpreted feature importances to identify key risk factors for severe COVID-19
- Libraries: `Pandas`, `Numpy`, `Scikit-learn`, `Matplotlib`, `Seaborn`

**Key Takeaways**

- Demonstrated the application of random forests for predicting disease severity
- Highlighted the importance of feature selection and hyperparameter tuning

![Random_Forest](images/random_forest.png)

[Link to COVID-19 Random Forest Case Study notebook](https://github.com/dennisvdang/Springboard-Portfolio/blob/main/Case%20Studies/Random%20Forest%20(Covid%20Case%20Study)/RandomForest_casestudy_covid19.ipynb)

## Diabetes Prediction (Grid Search KNN Case Study)

**Objective**

- Optimize the hyperparameters of a K-Nearest Neighbors (KNN) classifier using grid search on the Pima Indians Diabetes dataset.

**Methodology**

- Loaded and preprocessed the Pima Indians Diabetes dataset and standardize the features.
- Implemented a loop to train KNN models with a range of neighbor values (1-9) and evaluated the training and test scores.
- Identified the optimal number of neighbors based on the maximum test score.
- Fit the KNN model with the optimal number of neighbors and evaluated its performance on the training and test sets.
- Plotted the confusion matrix and printed the classification report for the optimal model.
- Applied the grid search method to find the optimal number of estimators in a Random Forest model.
- Libraries: `Pandas`, `Scikit-learn`, `Matplotlib`

**Key Takeaways**

- Grid search is an effective technique for optimizing hyperparameters of machine learning models, such as the number of neighbors in KNN and the number of estimators in Random Forest.
- Identifying the optimal hyperparameters can significantly improve the model's performance on both the training and test datasets.
- Visualizing the model's performance, such as through confusion matrices and classification reports, provides valuable insights into the model's strengths and weaknesses.

[Link to Diabetes Prediction Case Study notebook](https://github.com/dennisvdang/Springboard-Portfolio/blob/main/Case%20Studies/Grid%20Search%20KNN%20Case%20Study/GridSearchKNN_Case_Study.ipynb)

## London Housing Price Forecasting (Time Series Analysis/EDA Case Study)

**Objective**

- Analyze trends in London's housing market and forecast future prices

**Methodology**

- Conducted exploratory data analysis (EDA) to understand the impact of the 2008 financial crisis on London's housing market
- Applied statistical tests to explore the relationship between pre-crisis prices and crisis recovery time
- Employed time series models (ARIMA, SARIMA) and Random Forest to forecast property values
- Evaluated model performance using MSE and MAE
- Libraries: `Pandas`, `Numpy`, `Statsmodels`, `Matplotlib`, `Seaborn`

**Key Takeaways**

- Identified trends and patterns in London's housing market over time
- Demonstrated the application of time series modeling for forecasting

[Link to London Housing Case Study notebook](https://github.com/dennisvdang/Springboard-Portfolio/blob/main/Case%20Studies/London%20Housing%20Case%20Study/Springboard%20London%20Housing%20Case%20Study%20-%20Tier%203.ipynb)

## Wine Quality Prediction (Linear Regression Case Study)

**Objective**

- Predict alcohol levels in wine using regression analysis and build an accurate model

**Methodology**

- Performed univariate and multivariate analysis to iterate towards an accurate model
- Utilized EDA to visualize correlations and inform model selection
- Developed multiple linear regression models, iterating to improve accuracy and reduce redundancy
- Evaluated models based on R-squared, AIC, and BIC metrics
- Libraries: `Pandas`, `NumPy`, `Matplotlib`, `Seaborn`, `Statsmodels`, `Scikit-learn`

**Key Takeaways**

- Importance of iterative model development and feature selection
- Demonstrated the application of linear regression in predicting continuous variables
- Identified the most elegant and economical model (rModel4) using a few predictors effectively

[Link to Linear Regression Case Study notebook](https://github.com/dennisvdang/Springboard-Portfolio/blob/main/Case%20Studies/Linear%20Regression%20(Wine%20Quality%20Case%20Study)/Springboard%20Regression%20Case%20Study%20-%20the%20Red%20Wine%20Dataset%20-%20Tier%203.ipynb)

## Heart Disease Prediction (Logistic Regression Case Study)

**Objective**

- Build a logistic regression model to predict the presence of heart disease using patient health data

**Methodology** 

- Introduced logistic regression as a fundamental classification algorithm
- Covered key concepts like classification, model evaluation, discriminative vs generative classifiers
- Performed data preprocessing (handling missing values, encoding categorical variables)
- Split the data into training and testing sets
- Built and evaluated logistic regression models using scikit-learn
- Explored model tuning and evaluation metrics (accuracy, precision, recall, ROC curves)
- Visualized decision boundaries and interpreted model coefficients
- Libraries: `Pandas`, `Scikit-learn`, `Matplotlib`, `NumPy`

**Key Takeaways**

- Logistic regression is a simple yet effective algorithm for binary classification problems
- Importance of proper data preprocessing and model evaluation for classification tasks
- Logistic regression provides interpretable models and discriminative decision boundaries
- Need to consider multiple evaluation metrics beyond accuracy for imbalanced datasets

[Link to Logistic Regression Case Study notebook](https://github.com/dennisvdang/Springboard-Portfolio/blob/main/Case%20Studies/Logistic%20Regression%20(Heart%20Disease%20Case%20Study)/Logistic%20Regression%20Advanced%20Case%20Study.ipynb)

## Passenger Survival Prediction (Gradient Boosting Case Study)

**Objective**

- Explore the concept of gradient boosting using decision trees as base predictors to predict passenger survival in the Titanic dataset

**Methodology**

- Utilized the Titanic dataset to demonstrate the application of gradient boosting for binary classification
- Preprocessed the dataset, handling missing values and encoding categorical variables
- Demonstrated the process of fitting a series of decision trees on residual errors to improve predictions
- Evaluated model performance with multiple learning rates and calculated the ROC curve
- Libraries: `Pandas`, `NumPy`, `Scikit-learn`, `Matplotlib`

**Key Takeaways**

- Gradient boosting can significantly improve model performance in predicting passenger survival
- Importance of tuning hyperparameters, such as learning rate and number of estimators, to optimize model performance
- Demonstrated the effectiveness of gradient boosting in handling complex datasets with a mix of numerical and categorical features

[Link to Gradient Boosting Case Study notebook](https://github.com/dennisvdang/Springboard-Portfolio/blob/main/Case%20Studies/Gradient%20Boosting/Gradient%20Boosting%20Case%20Study.ipynb)

## Flight Delay Prediction (Bayesian Optimization Case Study)

**Objective**

- Use Bayesian Optimization to tune hyperparameters of a LightGBM model for flight delay prediction

**Methodology**

- Loaded and preprocessed the flight delay dataset, handling missing values and encoding categorical features.
- Evaluated the LightGBM model with given hyperparameters using cross-validation.
- Set up the Bayesian Optimization process using the `BayesianOptimization` library, specifying the hyperparameter search space.
- Performed Bayesian Optimization to find the optimal hyperparameters that maximize the AUC (Area Under the Receiver Operating Characteristic Curve) metric.
- Trained the final LightGBM model with the optimal hyperparameters obtained from Bayesian Optimization.
- Evaluated the final model's performance on the test set and compared it with a majority class baseline.
- Libraries: `Pandas`, `NumPy`, `LightGBM`, `Scikit-learn`, `Bayesian Optimization`, `Matplotlib`

**Key Takeaways**

- Bayesian Optimization is an effective technique for optimizing hyperparameters of complex machine learning models, such as LightGBM.
- Visualizing the model's performance using metrics like AUC, confusion matrix, and accuracy provides insights into the model's strengths and weaknesses.

[Link to Bayesian Optimization Case Study notebook](https://github.com/dennisvdang/Springboard-Portfolio/blob/main/Case%20Studies/Bayesian%20Optimization%20Case%20Study/Bayesian_Optimization_Case_Study_Cleaned.ipynb)

## Sales Forecasting (Time Series Forecasting with ARIMA Case Study)

**Objective**

- To analyze the sales data of Cowboy Cigarettes from 1949 to 1960 and predict future sales using time series forecasting with the ARIMA model.

**Methodology**

- Loaded and explored the historical sales data of Cowboy Cigarettes.
- Performed data cleaning and transformation, including log transformation to stabilize the variance.
- Conducted exploratory data analysis (EDA) to understand the trend, seasonality, and noise in the sales data.
- Utilized the Augmented Dickey-Fuller test to check for stationarity and applied differencing to achieve a stationary time series.
- Employed the ARIMA model for time series forecasting, optimizing the model parameters (p, d, q) based on the Akaike Information Criterion (AIC).
- Forecasted future sales for the next two years and visualized the original data along with the forecasts.

**Key Takeaways:**
- The ARIMA model effectively captured the underlying trend and seasonality in Cowboy Cigarettes' sales data, providing a close fit to the historical data.
- Forecasting revealed an increasing trend in sales, suggesting a growing demand for Cowboy Cigarettes.
- The case study highlighted the importance of time series decomposition and the capability of ARIMA models in forecasting future trends based on historical data.
- Libraries: `Pandas`, `NumPy`, `Matplotlib`, `Seaborn`, `Statsmodels`

[Link to Time Series Analysis and Forecasting with ARIMA Case Study notebook](https://github.com/dennisvdang/Springboard-Portfolio/blob/main/Case%20Studies/Time%20Series%20Case%20Study/Cowboy%20Cigarettes%20Case%20Study%20-%20Tier%203.ipynb)

# Statistical Foundations

Summaries of case studies that explore and apply fundamental statistical techniques and mathematical principles, without necessarily building predictive models.

## Cosine Similarity

**Objective**

- Use cosine similarity to compare numeric data and text datasets

**Methodology**

- Calculated similarity measures for sentences/paragraphs
- Libraries: `NumPy`, `Pandas`, `Matplotlib`, `Scipy`, `Scikit-learn`

**Key Takeaways**

- Cosine similarity effective for comparing numeric and text data
- Applicable in NLP and recommendation systems

[Link to Cosine Similarity Case Study notebook](https://github.com/dennisvdang/Springboard-Portfolio/blob/main/Case%20Studies/Cosine%20Similarity/Cosine_Similarity_Case_Study.ipynb)

## Euclidean and Manhattan Distance

**Objective**

- Demonstrate calculation and comparison of Euclidean and Manhattan distances

**Methodology**

- Visualized distribution of distances through histograms
- Highlighted application in data science, foundational for PCA
- Libraries: `Pandas`, `NumPy`, `Matplotlib`

**Key Takeaways**

- Euclidean and Manhattan distances have different behaviors

[Link to Euclidean and Manhattan Distance Case Study notebook](https://github.com/dennisvdang/Springboard-Portfolio/blob/main/Case%20Studies/Euclidean%20and%20Manhattan%20Distance/Euclidean_and_Manhattan_Distances_Case_Study.ipynb)

## Frequentist Inference

**Objective**

- Apply Frequentist inference to real-world data, addressing practical business questions for a hospital

**Methodology**

- Emphasized statistical concepts like z-statistic, t-statistic, Central Limit Theorem, and confidence intervals
- Explored the Central Limit Theorem and its implications
- Estimated population mean and standard deviation from a sample
- Calculated confidence intervals
- Libraries: `Pandas`, `NumPy`, `Matplotlib`

**Key Takeaways**

- Demonstrated the application of Frequentist inference in making data-driven decisions
- Highlighted the importance of statistical concepts in real-world scenarios

[Link to Frequentist Inference Case Study notebook (Part 1)](https://github.com/dennisvdang/Springboard-Portfolio/blob/main/Case%20Studies/Frequentist%20Inference/Frequentist%20Inference%20Case%20Study%20-%20Part%20A%20(3).ipynb)
[(Part 2)](https://github.com/dennisvdang/Springboard-Portfolio/blob/main/Case%20Studies/Frequentist%20Inference/Frequentist%20Inference%20Case%20Study%20-%20Part%20B%20(2).ipynb)

# Summary of Mini Projects

## API Mini Project

**Objective**

- Explore the use of APIs for data collection and integration in data analysis workflows

**Methodology**

- Demonstrated making API requests, handling authentication, and parsing JSON responses
- Collected data from the GitHub API and performed basic analysis
- Libraries: `Requests`, `Pandas`, `Matplotlib`

**Key Takeaways**

- APIs enable access to vast amounts of data for analysis
- Python libraries simplify API interactions and data manipulation

[Link to Mini Project](https://github.com/dennisvdang/Springboard-Portfolio/blob/main/Mini%20Projects/api_data_wrangling_mini_project.ipynb)

## SQL Mini Project

**Objective**

- Demonstrate the use of SQL for data manipulation, aggregation, and analysis

**Methodology**

- Performed various SQL queries on a sample database (filtering, joining, grouping, sorting)
- Showcased SQL's power in handling complex data queries and transformations
- Libraries/Tools: `SQLite`, `Pandas`, `MySQL`, `PHPMyAdmin`

**Key Takeaways**

- SQL is a powerful tool for data manipulation and analysis
- Proficiency in SQL and SQL libraries in Python is essential for working with relational databases

[Link to Mini Project](https://github.com/dennisvdang/Springboard-Portfolio/blob/main/Mini%20Projects/sql_project.sql)

# Capstone

## Guided Capstone

**Objective**

- Complete a comprehensive data science project covering all stages of the data science lifecycle

**Methodology**

- Collaborated with a team to define project scope, objectives, and deliverables
- Conducted extensive EDA to gain insights and inform modeling
- Built and evaluated multiple machine learning models (regression, classification, clustering)
- Communicated findings through visualizations, reports, and presentations
- Libraries: `Pandas`, `Numpy`, `Scikit-learn`, `Matplotlib`, `Seaborn`

**Key Takeaways**

- Hands-on experience with the complete data science lifecycle
- Importance of collaboration, communication, and project management in data science

[Link to Capstone Project](https://github.com/dennisvdang/Springboard-Portfolio/tree/main/Springboard%20Guided%20Capstone)
