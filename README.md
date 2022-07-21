# Final_project


## Selected Topic

***Direct Bank Marketing***

## Reason for Selecting Topic

* Machine learning models can help improve direct marketing campaigns from the bank to target potential future customers
* This information can be used by oher banks or businneses to determine the efficency of direct marketing campaigns.

## Description of the Data Source

* The data is related with direct marketing campaigns of a Portuguese banking institution. 
* The marketing campaigns were based on phone calls. 
* The dataset we are using is [bank-full.csv](/bank-full.csv) with all examples and 17 inputs, ordered by date (older version of this dataset with less inputs).
* Number of instances= 45211 and Number of Attributes=17

## Machine Learning model selected

* Random Forest
* Logistic Regression

## Questions we hope to answer

* The classification goal is to predict if the client will subscribe a term deposit.
* Which demographic variables have the most importance while determining whether the client subscribes or not?

## Communication protocols 

**The team will comunicate in three different ways:**

* Slack Channel (Final-Project-Bank-Marketing-Data)
* Zoom (meetings during class schedule)
* Extra Zoom meetings when needed.

## Description of the data exploration and analysis phase of the project

**Pre-processing Data**
* Jupyter Notebook 
* Scripts in Jupyter dependant on Pandas and SQL engine relational database**

**Pandas used for preliminary data preprocessing**

* Read in raw .cvs data and preprocessed for model input
* Clean the data to remove nulls, irrelevant data columns, convert string to numerical values, create bins of numerical data ranges to reduce noise

**Feature selection**

* Dropped balance and contact columns
* Converted strings to value
* Grouping 

    1. age_group = ["<18","18-28","28-38",">38"]	
    2. duration_group = ["<103","103-180","180-319",">319"]

**Training and Testing Classification**

* Training 75%
* Testing 25% 	
    
**SQL engine**

* SQL Lite : Join Features and Targets using Primary keys
* Tables created, inner join function used to bridge tables listed below

    1. Table 1 - Information : Features or dependent variables  
    2. Table 2 - Outputs : Target or independent variables

## Description of preliminary feature engineering and preliminary feature selection, including decision-making process 

* We will use SQLite to build our database and begin running machine learning models through linear regression and random forest.  

* Our target feature "y" indicates whether a client subscribed by making a term deposit. We will use this target to train and test the data set.

## Explanation of model choice, incluing benefits and limitations

* Random forest can be effective at reducing the risk of overfitting a training model and improve accuracy, but a large number of decision trees can also 
make the model slower and possibily ineffective for real-time predictions.

* Linear regression performs well for linearly separable data and is easy to train, but can be prone to overfitting and there is an assumption of the linear
relationship between dependent and independent variables.

## Dashboard

**The Dashboard can be reviewed using the following link**
- https://public.tableau.com/app/profile/hans.feddersen/viz/FP_Dash_2/Dashboard2?publish=yes

### Description of tools and interactive elements
* Planning to use Tableau to create interactive charts that will address which demographic variables have the most importance while determining whether the client subscribes or not.

* [Path to Google Slides][(/https://docs.google.com/presentation/d/1ndyXhv82vYUYCNXBWogu9qnl2aCWIHBR6GyQMjSj1Qo/edit#slide=id.g13d12802ede_1_17)](https://docs.google.com/presentation/d/1ndyXhv82vYUYCNXBWogu9qnl2aCWIHBR6GyQMjSj1Qo/edit#slide=id.g13d12802ede_1_17)
