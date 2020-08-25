## Project 3 - Housing Price Prediction

#### Overview

We will be using a housing dataset for Ames, Iowa from a [Kaggle Competition](http://kaggle.com/c/house-prices-advanced-regression-techniques/overview) to predict housing prices.  The challenge with this project is that it has been preporcessed with 79 variables/features of a residential home.  Using creative feature enigineering in combination with advanced regression our goal is to predict the final price of each home.

#### Step by Step
We will need to load the data and remove the non-essential features and combined redudant features.  And then further split the dataset into quantitative features we choose and create a target variable of a median value from the sales price.  Our feature assumptions include: the higher the number of bedrooms and bathrooms, higher square footage, higher lot size, recency of a remodel, then the higher the price.  Features such as the type of garage, whether or not there is a basement, type of zoning will be explored as to whether or not those are contributing features to a price.  We will use Pandas in Jupyter Notebook for splitting and removing data, and then load the data into Postgres.

We will explore that data using Matplotlib to show scatterplots and histograms to visualize relationships and correlations between the features.  As well as to identify any outliers.  We will also use a correlation matrix to standardize the different variables.  Using regression analysis with sklearn r2_score to help predict the mean of the target variable.

The datasets are already split into training and testing to test the balance between bias and variance.  And then review the training and test scores for a decision tree regressor for learning curves with an increasing 'max depth' parameter.  After determining the best maximum depth for the best validation score we will have our optimal model.

We will then evaluate the optimized model using a grid search parameter for fitting the dataset to the different values.  Then use K-fold cross validation to ensure the model is well trained by averaging the K scores obtained.

Our final procces will be using a decsision tree algorithm with the grid search technique and 'max_depth' parameter.  The decision tree regressor can then respond with a prediction for the target variable-median value of a home.

#### Requirements
1. *Find a problem worth solving, analyizing, or visualizing.*

  Utlizing this dataset as a case study will help in developing skills to make housing predictions on other datasets.  Housing predictions can aid those who want to know when     they should be buying and/or selling a home.  Using this information can also lead to an analysis on wealth inequality as to whether or not gaps are widening between those who   are or are not able to purchase a home.  Visualizations would help identify areas where features and trends are stronger for higher prices, who that may affect, and relocation   trends.

2. *Use ML in the context of technologies learned.*
  
  We will be using linear regression and advanced regression techniques learned like random forest and gradient boosting.

3. *You muse use: Scikit-Learn and/or another machine learning library.*

  We will be using Scikit-Learn and Numpy.

4. *You must use at least two of the following: Python Pandas, Python Matplotlib, HTML/CSS/Bootstrap, JavaScript Plotly, JavaScript D3.js, JavaScript Leaflet, SQL Database, MongoDB Database, GoogleClould SQL, Amazon AWS, Tableau.*

  We will be using Python Pandas, Python Matplotlib, and Tableau.

5. *Host application using Heroku or a tool of your choice.*

  We will be using Jupyter Notebook and Public Tableau.

6. *Prepare a 15-minute data deep-dive or infrastructure walkthrough that shows machine learning in the context of what we've already learned.*
  
  We will break down a walkthrough into three parts with 5 minutes each to present the machine learning that we have learned.

#### Resources
* https://towardsdatascience.com/machine-learning-project-predicting-boston-house-prices-with-regression-b4e47493633d
* https://towardsdatascience.com/feature-engineering-for-machine-learning-3a5e293a5114
* https://medium.com/@lhessani.sa/what-is-the-difference-between-training-and-test-dataset-91308080a4e8
* 21-Machine Learning Activities
  * Day 2: 09-Ins_GridSearch, 1-Stu_GridSearch, Ins_DecisionTrees_Graphviz
  * Day 3: 02-Evr_First_Neural_Network, 06-Ins_Saving_Models, 08-Ins_Kmeans, 09-Stu_Kmeans
  
