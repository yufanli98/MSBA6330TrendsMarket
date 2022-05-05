# Customer Churn Prediction in OTT Platforms
This project repository is created in partial fulfillment of the requirements 
for the Big Data Analytics course offered by the Master of Science in Business Analytics 
program at the Carlson School of Management, University of Minnesota

# Project Description
The objective of this project is to predict “customer churn” which is if a listener is likely to cancel their subscription. Our goal is to identify these customers via their interactions with the website. The dataset contains 18 features which can be used to predict the probability of churn. 

# Data description: 
This is a public dataset named Million Song Dataset and can be downloaded under json format prepared by Udacity. It contains 18 columns which have the information of customers(gender, name, etc.) and API events(login, playing next song, etc.) The experiment period is from 2018–10–01 to 2018–12–01. The data set is a 12 GB user log data which is hosted on a AWS S3 repository.  

## To access the dataset:
Dataset is available on S3 and can be accessed as below:

#### Step1: Create spark session
spark = SparkSession \
         .builder \
         .appName("Sparkify") \
         .getOrCreate()

#### Step2: Read in sparkify dataset
full_data = "s3n://udacity-dsnd/sparkify/sparkify_event_data.json"
mini_data = "s3n://udacity-dsnd/sparkify/mini_sparkify_event_data.json"

df = spark.read.json(full_data)



# Target audience: 
The target audience of our analysis would be digital music service firms and their stakeholders who would be interested in preventing customer churn. 

# Big Data Tools Used: 
Ingestion, ETL, exploration, Analysis: AWS S3, Databricks(Spark)
Visualization: AWS quicksight







