
# Lab Overview
This lab we add **Database class** for two tables can be joined together. We have cities and countries tables in this lab.

# Project Structure
    oop_lab3/
    │
    ├── Cities.csv # for cities table
    ├── Countries.csv # for Countries table
    ├── data_processing.py # main program
    └── README.md
---
# Design Overview
### **explanation for each class**
---
### DataLoader 
    loads CSV files into lists of dictionaries  

**Attributes**
- base_path : Directory where CSV files are located.

**Methods**
- load_csv(filename) : Reads a CSV file and returns a list of dictionaries.

---
### DB
    Stores multiple Table objects.

**Attributes**
- table : List of tables stored in the database.

**Methods**
- insert(table) : Adds a table to the DB.  
- search(name) : Retrieves a table by its name.

---
### Table
    a dataset and provide operations on the data.

**Attributes**
- table_name : Name of the table.  
- table : List of dictionaries.

**Methods**
- filter(condition) : Returns a new table that match the condition.  
- aggregate(function, key) : Applies an aggregation function to values in a specific list.  
- join(other, key) : Joins two tables and returns a new table.  
- __ str __() : Returns a string of the table.

---
# How to test and run your code
you can run the file data_processing.py and check if the result of test case match the table in Cities.csv and Countries.csv files


