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
Dimensionality reduction: PCA (principal component analysis) and LDA (linear discriminant analysis).   
Feature selection:   
- Filter: variance threshold, pearsonr correlation, chi-square test  
- Wrapper: recursive feature elimination  
- Embedded: L1, L2  

## Model training and Prediction
This step will select multiple machine learning models to train. 
#### * Supervised learning
Data with labeling 
- Regression： LinearRegression, DecisionTreeRegression, 
- Classification: LogisticRegression, Support Vector Machine (SVM)
#### * Unsupervised learning
Data without labeling
- Clustering

## Model evaluation
There has two methods to select suitable model
#### * Regularization   
#### * Cross validation  
Splitting the data by training set (60%), validation set (20%) and testing set (20%).
- training set: model training  
- validation set: model selection  
- testing set: final model evaluation
