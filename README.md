# SQL Data-WareHouse Projects

## Hello and welcome , Hrithik Saxena this side

# About the project and why ? 

I am creating this project as the part of my data engineer/analyst journey . where i am building the project SQL Data-warehouse.Where i am using the Medallion Architecture. All thanks to my teacher code with baraa giving me the  hands on exposure in this project to put my skills some test. In medallion architecture 
we have have three layers bronze silver gold layers . I will be working on that ... 

<img width="20" height="20" alt="image" src="https://github.com/user-attachments/assets/2f9817ad-02cd-4b16-b8d1-806110c7bcff" /> Bronze Layer

###  About this layer 

=> 1. Before building anything we analyze it. We understand the source system then we ask question about the source of the data from it was coming. then we do data ingestion all the coding part  take all the unprocessed data from the source system to the warehouse . then we do the schema checks data validation . After this we do git versioning .


## As in first step 


 1> We start with discussion with the source team asking them the right question About the source . Asking the right question about the source system is the crucial part . Question like 

 ===> Business Context and ownership 
 Q1. Who owns the data? , Q2 What business process it support?, Q3 System and Data Documentation? , Q4 Data Model and Data Catalog? 

 ===> Architecture and technology stack 
 Q1 How is data stored? (SQL server , Azure , AWS , Oracle) , Q2 What are the integration Condition ? (API Kafka , Direct db) , 

 ===> Extract and load 
 Q1 Incremental and full Load ?  Q2 Data scope and historical need? , Q3 What is the expected size of the extracts? , Q4 Are there any  data volume limitation ? , Q5 How to avoid impacting the source system performance ? , Q6 Authentication and Authorization (tokens , ssh , keys VPN , IP Whitelisting) 

=> after that  we start defining the table in bronze layer and then we do the bulk defining. Basically the bulk insert means we upload the massive amount the data directly from the .csv and .txt files into the database . 


==> After writing all the ddl commands we init the bronze layer load the unprocessed data ; 

 
<img width="30" height="30" alt="image" src="https://github.com/user-attachments/assets/b4b8c48a-5bcb-4b06-a26e-c9489915f1b7" /> Silver Layer

### About this layer 

Here in this the process start with understanding the data and exploring the data after that we clean the data we check quality of bronze. After this we check the data correctness. After this we do data versioning and commenting .

===> First we make the integration model Checking how the tables are related and matching the columns to the related columns.

===> after this we clean and load it is important because before transformation we need to clean it.
===> Then we go with quality check procedure like checking the null values in primary key we check the duplicates in our data 

