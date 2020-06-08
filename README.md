## Udacity Data Engineer Nano Degree Project-2

## Data Modeling with Cassandra

# 1.Overview

A startup called Sparkify wants to analyze the data they've been collecting on 
songs and user activity on their new music streaming app. The analysis team is 
particularly interested in understanding what songs users are listening to. Currently, 
there is no easy way to query the data to generate the results, since the data reside 
in a directory of CSV files on user activity on the app.

To help in getting needed info, we have to create an Apache Cassandra database, then query on song play data. The raw data is in a directory of CSV files, and we will build a ETL pipeline to transform the raw data into the Apache Cassandra database.

#  2.Project Steps
<ul>


<li><a href="#1"> Create an Apache Cassandra database which can create queries on song play data to answer the questions.</a></li>

<li><a href="#2"> Create a streamlined CSV file to model and insert data into Apache Cassandra tables, using the ETL pipeline that transfers data from a set of CSV files within a directory. </a></li>

<li><a href="#3"> Test the database by running queries given by the analytics team from Sparkify.</a></li>

</ul>


<a id='1'></a>
### 2.1 Model the data by creating tables in Apache Cassandra to run queries.

* Process the `event_datafile_new_1.csv` dataset to create a denormalized dataset
* Write Apache Cassandra `CREATE KEYSPACE` and `SET KEYSPACE` statements.
* Develop `CREATE` statement for each of the tables to address each question.
* Load the data with `INSERT` statement for each of the tables.
* Include `IF NOT EXISTS` clauses in `CREATE` statements to create tables only if the tables do not already exist. 



<a id='2'></a>
### 2.2 Create a streamlined CSV file to model and insert data into Apache Cassandra tables.

* Implement the logic in section Part I of the notebook template to iterate through each event file in `event_data` to process and create a new CSV file in Python.

* Make necessary edits to Part II of the notebook template to include Apache Cassandra `CREATE` and `INSERT` statements to load processed records into relevant tables in the existing data model.

<a id='3'></a>
### 2.3 Test the database.

* Test by running the proper `SELECT` statements with the correct `WHERE` clause,after running the queries on the  database.
