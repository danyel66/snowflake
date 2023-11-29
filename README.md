# snowflake
Data Cleaning in Snowflake: Techniques to Clean Messy Data

This code sets up a Snowflake database and a table named "CUSTOMERS." 
It manually loads data into the table, performs various data manipulations, and handles missing data. 
It then identifies inactive customers, handles duplicated records, and creates a view called "CUSTOMERS_VW" to store information about inactive customers. 
Finally, it queries the view to retrieve and export the list of inactive customers in ascending order by ID into a CSV file.

Here's a summary of the key steps:

Database and Table Creation:

Creates a Snowflake database named "SNOWFLAKE."
Defines a table named "CUSTOMERS" with various columns.
Data Loading:

Manually inserts data into the "CUSTOMERS" table.
Data Manipulation:

Uses SQL functions like TRIM(), SPLIT_PART(), TO_DATE(), and DATEDIFF() to manipulate and extract information from the data.
Identifying Inactive Customers:

Determines the number of days since the last transaction and identifies inactive customers (days since last transaction > 90).
Handling Missing Data:

Deletes rows with missing email data.
Imputes missing company data with "NA."
Handling Duplicated Data:

Identifies and eliminates duplicate customer records based on email, keeping the record with the latest transaction date.
View Creation:

Creates a view named "CUSTOMERS_VW" containing information about inactive customers.
Exporting Data:

Queries the view to retrieve inactive customer data and exports the results to a CSV file, ordered by ascending customer ID.




