## Crowdfunding ETL Mini Project ##
This project involves the extraction, transformation, and loading (ETL) of crowdfunding campaign data. The data is processed from Excel files to create 
multiple DataFrames for categories, subcategories, campaigns, and contacts. The final data is imported into a PostgreSQL database.

# Table of Contents
1. Overview
2. Project Workflow
   
   a. Create the Category and Subcategory DataFrames
   b. Create the Campaign DataFrame
   c. Create the Contacts DataFrame
   d. Create the Crowdfunding Database

# Overview
This project focuses on transforming crowdfunding data stored in Excel format into multiple clean DataFrames, which are then exported as CSV files and imported 
into a PostgreSQL database. The project is divided into the following sections:

* Creating category and subcategory DataFrames.
* Creating the campaign DataFrame.
* Extracting and transforming contact data.
* Designing and creating a relational database.

# Project Workflow

1. Create the Category and Subcategory DataFrames
Category DataFrame: Extracts unique categories from crowdfunding.xlsx, assigning each a category_id and category name. The resulting DataFrame is exported
as category.csv. Subcategory DataFrame: Extracts unique subcategories, assigning each a subcategory_id and subcategory name.
The resulting DataFrame is exported as subcategory.csv.

2. Create the Campaign DataFrame
Extracts and transforms the campaign data from the Excel file, creating columns for cf_id, contact_id, description, goal, pledged, outcome, backers_count,
launch_date, end_date, etc. Converts date fields to datetime and exports the final DataFrame as campaign.csv.

3. Create the Contacts DataFrame
You can choose between two approaches to extract and transform the contact data:

Using Python Dictionary Methods
Converts rows to dictionaries, extracting values and splitting names into first and last names.


4. Create the Crowdfunding Database
Create an Entity Relationship Diagram (ERD) and a schema using QuickDBD.
Use the schema to define the database in PostgreSQL, specifying primary and foreign keys.
Import the CSV files (category.csv, subcategory.csv, campaign.csv, and contacts.csv) into the database.
