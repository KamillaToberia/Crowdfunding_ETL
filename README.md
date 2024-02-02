This application uses Pandas, JSON, PostGreSQL, and QuickDBD to create and visualize a crowdfunding database complete with contact info (names and emails) from backers.

1. Extracts and transforms excel data from contacts.xlsx and crowdfunding.xlsx to create a campaign dataframe
2. The campaign dataframe is then converted to csv as campaign.csv
3. The contact dataframe is created by iterating through the comma-separated data within the contacts.xlsx file and creating a dictionary by using list comprehensions.
4. A crowdfunding database is created by connecting keys from the campaign.csv file to the data in the category.csv, subcategory.csv, and contacts.csv files
5. The database is exported as a Postgres file named crowdfunding_db_schema.sql
6. A a new Postgres database named crowdfunding_db is created using the schema from the above step
7. Validates data by running SELECT statements
