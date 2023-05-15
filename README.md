# Crowdfunding_ETL

## Project 2 - Crowdfunding_ETL 
### Group 1 - Kirby Judd, Matthew Siriani, Emily Washburn

# Background
For the ETL mini project, you will work with a partner to practice building an ETL pipeline using Python, Pandas, and either Python dictionary methods or regular expressions to extract and transform the data. After you transform the data, you'll create four CSV files and use the CSV file data to create an ERD and a table schema. Finally, you’ll upload the CSV file data into a Postgres database.

Since this is a one-week project, make sure that you have done at least half of your project before the third day of class to stay on track.

Although you and your partner will divide the work, it’s essential to collaborate and communicate while working on different parts of the project. Be sure to check in with your partner regularly and offer support

# Instructions
The instructions for this mini project are divided into the following subsections:

- Create the Category and Subcategory DataFrames
- Create the Campaign DataFrame
- Create the Contacts DataFrame
- Create the Crowdfunding Database

## Create the Category and Subcategory DataFrames

Create a Category DataFrame that has the following columns:

A "category_id" column that is numbered sequential form 1 to the length of the number of unique categories.
A "category" column that has only the categories.
Export the DataFrame as a category.csv CSV file.

Create a SubCategory DataFrame that has the following columns:

A "subcategory_id" column that is numbered sequential form 1 to the length of the number of unique subcategories.
A "subcategory" column that has only the subcategories.
Export the DataFrame as a subcategory.csv CSV file.

## Create the Campaign DataFrame
Create a Campaign DataFrame that has the following columns:

The "cf_id" column.
The "contact_id" column.
The “company_name” column.
The "blurb" column is renamed as "description."
The "goal" column.
The "goal" column is converted to a float datatype.
The "pledged" column is converted to a float datatype.
The "backers_count" column.
The "country" column.
The "currency" column.
The "launched_at" column is renamed as "launch_date" and converted to a datetime format.
The "deadline" column is renamed as "end_date" and converted to a datetime format.
The "category_id" with the unique number matching the “category_id” from the category DataFrame.
The "subcategory_id" with the unique number matching the “subcategory_id” from the subcategory DataFrame.
And, create a column that contains the unique four-digit contact ID number from the contact.xlsx file.
Then export the DataFrame as a campaign.csv CSV file.

## Create the Contacts DataFrame
Create a Contacts DataFrame that has the following columns:

A column named "contact_id" that contains the unique number of the contact person.
A column named "first_name" that contains the first name of the contact person.
A column named "last_name" that contains the first name of the contact person.
A column named "email" that contains the email address of the contact person
Then export the DataFrame as a contacts.csv CSV file.

We decided to use Option 1: Use Pandas to create the contacts DataFrame.

## Create the Crowdfunding Database
- We then created the Crowdfunding Database using QuickDBD to create the table schema.
- A database schema labeled, crowdfunding_db_schema.sql was created 
- A crowdfunding_db is created using the crowdfunding_db_schema.sql file.
- The database has the appropriate primary and foreign keys and relationships.
- Each CSV file is imported into the appropriate table without errors.
- The data from each table is displayed using a SELECT * statement.

## File locations
- The Database images are locate in the "Database Screenshots" folder.
- The main jupyter notebook "ETL_Mini_Project_KJudd_MSiriani_EWashburn.ipynb" is located in the second "Starter_Files" folder
- The starer csv and excel files are located within the Starter_Files folder in the "Resources" folder
- The campagin.csv and contacts.csv were also exported into the "Resources" folder
