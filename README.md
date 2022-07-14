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

## Description of the data exploration phase of the project
### Pre-processing Data
* We used Pandas to review the list of columns, non-null value counts and dtype of each column. We had zero null values and the data types were either
integer or object.
* We checked the values in the "contact" and "balance" columns and dropped both columns from the dataframe.
* We  transformed month names into integers by creating a new month_num column and dropped the month name column.
* We used LabelEncoder to transform object data into integers, including our target column "y".
* We binned and grouped data based on data in the columns of "duration" and "age." We created 4 groups/bins for each feature and then transformed the data back into 
integers. 

## Description of the analysis phase of the project 
### Description of preliminary feature engineering and preliminary feature selection, including decision-making process 
* We will use SQLite to build our database and begin running machine learning models through linear regression and random forest.  
* Our target feature "y" indicates whether a client subscribed by making a term deposit. We will use this target to train and test the data set.
### How was data split into training and testing sets?
### Explanation of model choice, incluing benefits and limitations
* Random forest can be effective at reducing the risk of overfitting a training model and improve accuracy, but a large number of decision trees can also 
make the model slower and possibily ineffective for real-time predictions.
* Linear regression performs well for linearly separable data and is easy to train, but can be prone to overfitting and there is an assumption of the linear
relationship between dependent and independent variables.

## Dashboard
### Description of tools and interactive elements
* Planning to use Tableau to create interactive charts that will address which demographic variables have the most importance while determining whether the client subscribes or not.
