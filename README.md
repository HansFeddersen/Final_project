# Final_project


## Selected Topic

***Direct Bank Marketing***

## Reason for Selecting Topic

* Machine learning models can help improve direct marketing campaigns from the bank to target potential future customers
* This information can be used by other banks or businesses to determine the efficency of direct marketing campaigns.

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

We tested three models 

* Random forest can be effective at reducing the risk of overfitting a training model and improve accuracy, but a large number of decision trees can also make the model slower and possibily ineffective for real-time predictions. 

![random forest accuracy](https://user-images.githubusercontent.com/99205688/180333859-74c4e9d7-bb07-4ae9-ab90-55d181062138.PNG)

![random forest classification](https://user-images.githubusercontent.com/99205688/180333844-ed464ee1-4d6a-4639-93d5-b150805a1f15.PNG)

* Logistic regression with standard scaler performs well for linearly separable data and is easy to train, but can be prone to overfitting and there is an assumption of the linear relationship between dependent and independent variables. 

![logistic regression](https://user-images.githubusercontent.com/99205688/180333826-564dd79b-513f-498e-b422-956603bff804.PNG)

After reviewing our dataset, we also decided to try SMOTTENN as a potential 3rd model.

* SMOTEENN performs well when the existing classes in a dataset aren't equally represented. In our dataset, the target feature of campign failures make up a much larger part of the dataset than the campaign successes. We used SMOTEENN to try to address this imbalance in our dataset. 

![SMOTENN](https://user-images.githubusercontent.com/99205688/180333881-1fe5be18-b48a-4037-a62d-469bd4e53b6d.PNG)

## Dashboard 

**The Dashboard can be reviewed using the following link:**
- https://public.tableau.com/app/profile/hans.feddersen/viz/FP_Dash_2/Dashboard2?publish=yes

### Description of tools and interactive elements
* Planning to use Tableau to create interactive charts that will address which demographic variables have the most importance while determining whether the client subscribes or not.

* [Path to Google Slides][(/https://docs.google.com/presentation/d/1ndyXhv82vYUYCNXBWogu9qnl2aCWIHBR6GyQMjSj1Qo/edit#slide=id.g13d12802ede_1_17)](https://docs.google.com/presentation/d/1ndyXhv82vYUYCNXBWogu9qnl2aCWIHBR6GyQMjSj1Qo/edit#slide=id.g13d12802ede_1_17)
