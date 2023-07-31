## Weekly challenge 3
1. A junior data analyst joins a new company. The analyst learns that SQL is heavily utilized within the organization. Why would the organization choose to invest in SQL? Select all that apply.
   ```
   • SQL can handle huge amounts of data.
   • SQL is a well-known standard in the professional community.
   ```
2. Your manager tasks you with analyzing a dataset and visually inspecting the data. Upon initial inspection you realize that this is a small dataset. What tool should you use to analyze the data?
   ```
   Spreadsheet
   ```
3. A data analyst creates many new tables in their company’s database. When the project is complete, the analyst wants to remove the tables so they don’t clutter the database. What SQL commands can they use to delete the tables?
   ```
   DROP TABLE IF EXISTS 
   ```
4. You are working with a database table named invoice that contains invoice data. The table includes a column for _invoice_date_. You want to remove duplicate entries for _invoice_date_. 
   <br/><br/>
   You write the SQL query below. Add a DISTINCT clause that will remove duplicate entries from the _invoice_date_ column. 
   ```
   SELECT DISTINCT(invoice_date)
   FROM invoice
   ```
   ```
   +---------------------+
   | invoice_date        |
   +---------------------+
   | 2009-01-01 00:00:00 |
   | 2009-01-02 00:00:00 |
   | 2009-01-03 00:00:00 |
   | 2009-01-06 00:00:00 |
   | 2009-01-11 00:00:00 |
   | 2009-01-19 00:00:00 |
   | 2009-02-01 00:00:00 |
   | 2009-02-02 00:00:00 |
   | 2009-02-03 00:00:00 |
   | 2009-02-06 00:00:00 |
   | 2009-02-11 00:00:00 |
   | 2009-02-19 00:00:00 |
   | 2009-03-04 00:00:00 |
   | 2009-03-05 00:00:00 |
   | 2009-03-06 00:00:00 |
   | 2009-03-09 00:00:00 |
   | 2009-03-14 00:00:00 |
   | 2009-03-22 00:00:00 |
   | 2009-04-04 00:00:00 |
   | 2009-04-05 00:00:00 |
   | 2009-04-06 00:00:00 |
   | 2009-04-09 00:00:00 |
   | 2009-04-14 00:00:00 |
   | 2009-04-22 00:00:00 |
   | 2009-05-05 00:00:00 |
   +---------------------+
   (Output limit exceeded, 25 of 354 total rows shown)
   ```
   What invoice_date is in row 17 of your query result?
   ```
   2009-03-14
   ```
5. You are working with a database table that contains customer data. The table includes columns about customer location such as _city, state,_ _country,_ and _postal_code_. The state names are abbreviated. You want to check for state names that are greater than 2 characters long. 
   <br/><br/>
   You write the SQL query below. Add a LENGTH function that will return any state names that are greater than 2 characters long.
   ```
   SELECT *
   FROM customer
   WHERE LENGTH(state)>2
   ```
   ```
   +-------------+------------+-----------+---------+-------------------+--------+--------+-----------+-------------+--------------------+------+----------------------+----------------+
   | customer_id | first_name | last_name | company | address           | city   | state  | country   | postal_code | phone              |  fax | email                | support_rep_id |
   +-------------+------------+-----------+---------+-------------------+--------+--------+-----------+-------------+--------------------+------+----------------------+----------------+
   |          46 | Hugh       | O'Reilly  |    None | 3 Chatham Street  | Dublin | Dublin | Ireland   |        None | +353 01 6792424    | None | hughoreilly@apple.ie |              3 |
   |          55 | Mark       | Taylor    |    None | 421 Bourke Street | Sidney | NSW    | Australia |        2010 | +61 (02) 9332 3633 | None | mark.taylor@yahoo.au |              4 |
   +-------------+------------+-----------+---------+-------------------+--------+--------+-----------+-------------+--------------------+------+----------------------+----------------+
   ```
   What country is in row 1 of your query result? _(Hint: you will have to scroll to the right with your mouse or track pad to locate the indicated column.)_
   ```
   Ireland  
   ```
6. In SQL databases, what data type refers to a number that does not contain a decimal?
   ```
   Integer 
   ```
7. A data analyst is working with product sales data. They import new data into a database. The database recognizes the data for product price as text strings. What SQL function can the analyst use to convert text strings to floats?
   ```
   CAST
   ```
8. A data analyst is cleaning survey data. The results for an optional question contain many nulls. What function can the analyst use to eliminate the null values from the results?
   ```
   COALESCE
   ```
9. You are working with a database table that contains customer data. The table includes columns about customer location such as _city, state,_ and _country_. The state names are abbreviated. You want to retrieve the first 2 letters of each state name. You decide to use the SUBSTR function to retrieve the first 2 letters of each state name, and use the AS command to store the result in a new column called _new_state_. 
   <br/><br/>
   You write the SQL query below. Add a statement to your SQL query that will retrieve the first 2 letters of each state name and store the result in a new column as _new_state_. 
   ```
   SELECT
   customer_id,
   SUBSTR(state,1,2)
   FROM
   customer
   ORDER BY
   state DESC
   ```
   ```
   +-------------+-------------------+
   | customer_id | SUBSTR(state,1,2) |
   +-------------+-------------------+
   |          25 | WI                |
   |          17 | WA                |
   |          48 | VV                |
   |          28 | UT                |
   |          26 | TX                |
   |           1 | SP                |
   |          10 | SP                |
   |          11 | SP                |
   |          47 | RM                |
   |          12 | RJ                |
   |           3 | QC                |
   |          29 | ON                |
   |          30 | ON                |
   |          18 | NY                |
   |          21 | NV                |
   |          33 | NT                |
   |          55 | NS                |
   |          31 | NS                |
   |          32 | MB                |
   |          23 | MA                |
   |          24 | IL                |
   |          22 | FL                |
   |          46 | Du                |
   |          13 | DF                |
   |          16 | CA                |
   +-------------+-------------------+
   (Output limit exceeded, 25 of 59 total rows shown)
   ```
   What customer ID number is in row 9 of your query result?
   ```
   47
   ```