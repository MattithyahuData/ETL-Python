# ETL-Python: Project Overview 
* Load Data into SQL Server, mySQL, and PostgreSQL using Python 3. 
    * [SQL Server Load](Code/ETL_SQLServer.ipynb)
    * [MySQL Load](Code/ETL_MySQL.ipynb)
    * [PostgreSQL Load](Code/ETL_PostgreSQL.ipynb)

## Resources Used
**Python 3.8.12  - SQL Server  - MySQL - PostgreSQL** 

[**Anaconda Packages:**](requirements.txt) **'pip install' :**
* SQL Server
    * **pandas, pyodbc**
* MySQL
    * **pandas, mysql.connector**
* PostgreSQL
    * **pandas, psycopg2**  

**Data sources:**
* [results](https://www.kaggle.com/martj42/international-football-results-from-1872-to-2017/data?select=results.csv) 
* [fifa_rankings](https://www.kaggle.com/tadhgfitzgerald/fifa-international-soccer-mens-ranking-1993now) 
* [fixtures](https://fixturedownload.com/feed/json/fifa-world-cup-2018)


## Data Collection
Download Sources: Kaggle | fixturedownload
* 


## Data Cleaning
After I had sraped and downloaded all the data I needed, I needed to clean it up so that it was usable for the model and analysis. I made the following changes and created the following variables:

*	Parsed numeric data out of salary 
*	Made columns for employer provided salary and hourly wages 
*	Removed rows without salary 
*	Parsed rating out of company text 
*	Made a new column for company state 
*	Added a column for if the job was at the company’s headquarters 
*	Transformed founded date into age of company 


## Exploratory data analysis 
I looked at the distributions of the data and the value counts for the various categorical variables. Below are a few highlights from the pivot tables. 

![alt text](https://github.com/PlayingNumbers/ds_salary_proj/blob/master/salary_by_job_title.PNG "Salary by Position")
![alt text](https://github.com/PlayingNumbers/ds_salary_proj/blob/master/positions_by_state.png "Job Opportunities by State")
![alt text](https://github.com/PlayingNumbers/ds_salary_proj/blob/master/correlation_visual.png "Correlations")


## Data Warehousing
AAAAAAAAAAAAAAAAAAAAAAAAA

*	Made a new column for company state 
*	Added a column for if the job was at the company’s headquarters 
*	Transformed founded date into age of company 


## Data Visualisation
AAAAAAAAAAAAAAAAAAAAAAAAA

*	Made a new column for company state 
*	Added a column for if the job was at the company’s headquarters 
*	Transformed founded date into age of company 

## Data Analytics
AAAAAAAAAAAAAAAAAAAAAAAAA

*	Made a new column for company state 
*	Added a column for if the job was at the company’s headquarters 
*	Transformed founded date into age of company 

## Business Intelligence
AAAAAAAAAAAAAAAAAAAAAAAAA

*	Made a new column for company state 
*	Added a column for if the job was at the company’s headquarters 
*	Transformed founded date into age of company 

## ML/DL Model Building 

First, I transformed the categorical variables into dummy variables. I also split the data into train and tests sets with a test size of 20%.   

I tried three different models and evaluated them using Mean Absolute Error. I chose MAE because it is relatively easy to interpret and outliers aren’t particularly bad in for this type of model.   

I tried three different models:
*	**Multiple Linear Regression** – Baseline for the model
*	**Lasso Regression** – Because of the sparse data from the many categorical variables, I thought a normalized regression like lasso would be effective.
*	**Random Forest** – Again, with the sparsity associated with the data, I thought that this would be a good fit. 

## Model performance
The Random Forest model far outperformed the other approaches on the test and validation sets. 
*	**Random Forest** : MAE = 11.22
*	**Linear Regression**: MAE = 18.86
*	**Ridge Regression**: MAE = 19.67

## Deployment 
In this step, I built a flask API endpoint that was hosted on a local webserver by following along with the TDS tutorial in the reference section above. The API endpoint takes in a request with a list of values from a job listing and returns an estimated salary. 

## Evaluation 
In this step, I built a flask API endpoint that was hosted on a local webserver by following along with the TDS tutorial in the reference section above. The API endpoint takes in a request with a list of values from a job listing and returns an estimated salary. 


# Data Source Link: 
[]()
