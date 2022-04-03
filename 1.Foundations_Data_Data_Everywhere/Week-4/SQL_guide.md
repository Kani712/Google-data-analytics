# SQL Guide: Getting started

Just as humans use different languages to communicate with others, so do computers. Structured Query Language (or SQL, often pronounced “sequel”) enables data analysts to talk to their databases. SQL is one of the most useful data analyst tools, especially when working with large datasets in tables. It can help you investigate huge databases, track down text (referred to as strings) and numbers, and filter for the exact kind of data you need—much faster than a spreadsheet can. 

If you haven’t used SQL before, this reading will help you learn the basics so you can appreciate how useful SQL is and how useful SQL queries are in particular. You will be writing SQL queries in no time at all.

**What is a query?**

> A query is a request for data or information from a database. When you query databases, you use SQL to communicate your question or request. You and the database can always exchange information as long as you speak the same language.

Every programming language, including SQL, follows a unique set of guidelines known as syntax. Syntax is the predetermined structure of a language that includes all required words, symbols, and punctuation, as well as their proper placement. As soon as you enter your search criteria using the correct syntax, the query starts working to pull the data you’ve requested from the target database.

The syntax of every SQL query is the same: 

* Use **SELECT** to choose the columns you want to return.

* Use **FROM** to choose the tables where the columns you want are located.

* Use **WHERE** to filter for certain information.

A SQL query is like filling in a template. You will find that if you are writing a SQL query from scratch, it is helpful to start a query by writing the SELECT, FROM, and WHERE keywords in the following format: 
                  
![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/MwhC5HMJRFKIQuRzCURSDw_754b0ed1d87441a298173d87c0bfdbf1_Select_From_Where.png?expiry=1649030400000&hmac=9Il0xfSDtZZl9TLvpve5sCQeo4Bb0-e7l0MOLAESL4Y)
                                   
Following this method each time makes it easier to write SQL queries. It can also help you make fewer syntax errors.

**Example of a query**
Here is how a simple query would appear in BigQuery, a data warehouse on the Google Cloud Platform.  

![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/vNz9GfCMQiGc_RnwjMIhfQ_1d09943b48924e6cbf9915e30f771d86_Screen-Shot-2020-11-11-at-4.25.17-PM.png?expiry=1649030400000&hmac=a_DhFAfOj3kacGd2ggqQ-_H9ynPZVjuo6nrxRweoouM)

The above query uses three commands to locate customers with the first name Tony:

1. **SELECT** the **column** named **first_name**

2. **FROM** a table named **customer_name** (in a dataset named **customer_data**)
   (The dataset name is always followed by a dot, and then the table name.)

3. But only return the data **WHERE** the **first_name** is Tony

The results from the query might be similar to the following:
