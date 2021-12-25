# Machine-Learning
Machine learning was a type of computer science which can automatically give a decisive result with empirical training by use of the data. It is divided by supervised learning and unsupervised learning.  
The flow of machine learning: Data exploration -> Data cleaning -> Feature engineering -> Model training -> Prediction -> Model evaluation.

## Data exploration
Visualizaing and understanding the data firstly.  
Several things need to do: Take a first image on distribution of data if it matches normal distribution or randomization. The condition about abnormal value, null value, mean value, standard deviation and unique feature. Also the relations between target variable and features.

## Data cleaning
Step is so important for prediction accuracy. Deleting and correcting error value, incomplete, incorrectly formatted or redundant data. Filling the null value by mean value. 

## Feature engineering
The step is extracting and transforming the most relevant features from raw data.  
#### * Single feature processing 
Nondimensionalization: standardization, min-max rescaling and normalization.  
Null value processing: Filling with mean, median  
One-hot encoding: using get_dummies from pandas. feature: [A1, A2, A3] -> feature_A1:[1, 0, 0], feature_A2:[0, 1, 0], feature_A3:[0, 0, 1]  
#### * Multiple features prcossing  
Feature selection:   
- Filter: variance threshold, pearsonr correlation, chi-square test  
- Wrapper: recursive feature elimination  
- Embedded: L1, L2  

## Model training and Prediction
This step will select multiple machine learning models to train. 
#### * Supervised learning
Data with labeling 
- Regression: As for a dataset of relevant data, It can be used to figure out the prediction and forecating task.  
  Ex: Weather Forecasting, Market Forecasting, Estimating life expectancy, Housing price prediction, Advertising Popularity Predction and Population Growth Prediction.  
  Most frequently method "LinearRegression", "DecisionTreeRegression", "RandomForestRegressor".  
  Reference: [Why we use Linear Regression to do the prediction?](https://medium.com/@sunyang19940702/why-we-use-linear-regression-to-do-the-prediction-6220df181047)
- Classification: As for a dataset of irrelvant data, It can be used to figure out the classification task.  
  Ex: Image Classification, Customer Retention, Diagnostics and Identity Fraud Detection.  
  Most frequently method "LogisticRegression", "Support Vector Machine (SVM)", "Decision Tree", "k-Nearest Neighbors", "Naive Bayes", "Boosting method".
#### * Unsupervised learning
Data without labeling  
- Dimensionality reduction: PCA (principal component analysis) and LDA (linear discriminant analysis).   
- Clustering:   
#### * Reinforcement Learning
- Games AI, Skill Acquisition, Learning Tasks, Real-time Decisions and Robot Navigation.  

## Model evaluation
There has two methods to select suitable model
#### * Cross validation  
Splitting the data by training set (60%), validation set (20%) and testing set (20%).
- training set: model training  
- validation set: model selection  
- testing set: final model evaluation   
#### * Evaluation index
- Regression: RMSE, R2, Cross-validation score
- Clissification: Accuarcy, Precision, Recall, F1 value. 
- Clustering:
