## Weekly challenge 3
1. Relational databases contain a series of tables connected to form relationships. Which two types of fields exist in two connected tables?
   ```
   Primary and foreign keys
   ```
2. What do metadata repositories do to make it simpler and quicker to use multiple data sources for analysis? Select all that apply.
   ```
   • Keep the metadata in an accessible form
   • Describe where data came from
   • Keep metadata in a common structure
   ```
3. Think about data as driving a taxi cab. In this metaphor, which of the following are examples of metadata? Select all that apply.
   ```
   • Make and model of the taxi cab
   • Company that owns the taxi
   • License plate number
   ```
4. What is the process that data analysts use to ensure the formal management of their company’s data assets?
   ```
   Data governance
   ```
5. What are some key benefits of using external data? Select all that apply.
   ```
   • External data provides industry-level perspectives.
   • External data has broad reach.
   ```
6. A school has a list of currently enrolled students with the columns first_name, last_name, and current_grade_level. They assign students to a guidance counselor by the first letter of their last name. (For example, counselor 1 will get A, B, and C; counselor 2 will get D, E, and F; and so on.) What would be the first step in organizing this data so the school can assign counselors to students?
   ```
   Sort last_name alphabetically in ascending order.
   ```
7. When writing a query, you add a WHERE condition to filter the set. What must you put around the value you are trying to match or search for?
   ```
   single quotes (‘)
   ```
8. You are working with a database table that contains customer data. The _state_ column lists the state where each customer is located. The state names are abbreviated. You want to find out which customers are located in the U.S. state of Florida (FL).
   <br/><br/>
   You write the SQL query below.
   <br/><br/>
   ```SELECT * FROM Customer```
   <br/><br/>
   What code would be added to return only customers located in FL?
   ```
   WHERE state = 'FL'
   ```