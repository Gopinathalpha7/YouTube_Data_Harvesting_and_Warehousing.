# YouTube Data Harvesting and Warehousing.

## Introduction 

* YouTube, the online video-sharing platform, has revolutionized the way we consume and interact with media. Launched in 2005, it has grown into a global phenomenon, serving as a hub for entertainment, education, and community engagement. With its vast user base and diverse content library, YouTube has become a powerful tool for individuals, creators, and businesses to share their stories, express themselves, and connect with audiences worldwide.

* This project extracts the particular youtube channel data by using the youtube channel id, processes the data, and stores it in the MongoDB database. It has the option to migrate the data to MySQL from MongoDB then analyse the data and give the results depending on the customer questions.


![Intro GUI](https://github.com/Gopinathalpha7/YouTube_Data_Harvesting_and_Warehousing./blob/3af3b25e63dd3d8b1928050135ebadbbf9b6f0e6/youtube%20data%20harvesting%20gui.png)


## Developer Guide 

### 1.Tools

* Virtual code.
* Jupyter notebook.
* Python 3.11.0 or higher.
* MySQL.
* MongoDB.
* Youtube API key.

### 2.Requirement Libraries to Install

* pip install google-api-python-client, pymongo, mysql-connector-python, sqlalchemy, pymysql, pymysql, pandas, numpy, 
  plotly-express, streamlit.
 
### 3.Import Libraries

**Youtube API libraries**
* import googleapiclient.discovery
* from googleapiclient.discovery import build

**File handling libraries**
* import json
* import re

**MongoDB**
* import pymongo

**SQL libraries**
* import mysql.connector
* import sqlalchemy
* from sqlalchemy import create_engine
* import pymysql

**pandas, numpy**
* import pandas as pd
* import numpy as np

**Dash board libraries**
* import streamlit as st
* import plotly.express as px

### 4. E T L Process

#### a) Extract data

* Extract the particular youtube channel data by using the youtube channel id, with the help of the youtube API developer console.

#### b) Process and Transform the data

* After the extraction process, takes the required details from the extraction data and transforms it into JSON format.

#### c) Load  data 

* After the transformation process, the JSON format data is stored in the MongoDB database, also It has the option to migrate the data to MySQL database from the MongoDB database.

### 5. E D A Process and Frame work

#### a) Access MySQL DB 

* Create a connection to the MySQL server and access the specified MySQL DataBase by using pymysql library and access tables.

#### b) Filter the data

* Filter and process the collected data from the tables depending on the given requirements by using SQL queries and transform the processed data into a DataFrame format.

#### c) Visualization 

* Finally, create a Dashboard by using Streamlit and give dropdown options on the Dashboard to the user and select a question from that menu to analyse the data and show the output in Dataframe Table and Bar chart.


## User Guide

#### Step 1. Data collection zone

* Search **channel_id**, copy and **paste on the input box** and click the **Get data and stored** button in the **Data collection zone**.

#### Step 2. Data Migrate zone

* Select the **channel name** and click the **Migrate to MySQL** button to migrate the specific channel data to the MySQL database from MongoDB in the **Data Migrate zone**.

#### Step 3. Channel Data Analysis zone

* **Select a Question** from the dropdown option you can get the **results in Dataframe format or bar chat format**.


## Video link

* Click the below Image

[![Intro GUI](https://github.com/Gopinathalpha7/YouTube_Data_Harvesting_and_Warehousing./blob/3af3b25e63dd3d8b1928050135ebadbbf9b6f0e6/youtube%20data%20harvesting%20gui.png)](https://www.linkedin.com/feed/update/urn:li:activity:7065793132247871488/)
