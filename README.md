# Data Modeling with Apache Cassandra
In this second **Udacity Data Engineering** project we must create an Apache Cassandra database for the music streaming startup **Sparkify**. This NoSql database will make queries on song play data faster for analysts to gain insights of their users' behavior. ```SparkifyKS``` is the name of the keyspace that contains three tables optimized to perform the following queries:

### 1. Table session_info
Query: 
Give me the artist, song title and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4

### 2. Table user_info
Query:
Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182

### 3. Table song_plays
Query: 
Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'


# Datasets and ETL

In this project, we work with one dataset: **event_data**. The directory of CSV files partitioned by date. Here are examples of filepaths to two files in the dataset:
````
event_data/2018-11-08-events.csv
event_data/2018-11-09-events.csv
````
The **Project_1B_ Project_Template.ipynb** jupyter notebook contains the ETL process and modeling of the data. In this notebook data from the **event_data** folder is extracted, transformed and loaded into the Apache Cassandra keyspace denormalized tables defined above. Queries are also executed in this notebook to verify primary key pairs and sort keys were accurate choices. 

