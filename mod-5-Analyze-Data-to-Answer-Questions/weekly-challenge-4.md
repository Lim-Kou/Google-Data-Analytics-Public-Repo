## Weekly challenge 4
1. A data analyst wants to calculate the number of rows that have a value of “shipped”. Which function could they use?
   ```
   =COUNTIF(G2:G30,”=shipped”)
   ```
2. You are working in a spreadsheet and use the SUMIF function in the following formula as part of your analysis.
   ```
   =SUMIF(D2:D10,”>=50”,E2:E10)
   ```
   Which part of this formula indicates the range of values to be added?
   ```
   E2:E10
   ```
3. You create a pivot table and want to add up the total of all cells for each row and column value in the pivot table. Which function in the values menu would you use to summarize the data?
   ```
   SUM
   ```
4. Which values of Date and Direction are used to calculate the value 450 in the following pivot table?

   <table><tbody><tr><td><p><span><span>N/A</span></span></p></td><td><p><span><span>N/A</span></span></p></td><td><p><span><em><span>Direction</span></em></span></p></td><td></td></tr><tr><td><p><span><em><span>Date</span></em></span></p></td><td><p><span><em><span>Values</span></em></span></p></td><td><p><span><span>Down</span></span></p></td><td><p><span><span>Up</span></span></p></td></tr><tr><td><p><span><span>2/3</span></span></p></td><td><p><span><span>MAX of A</span></span></p></td><td><p><span><span>300</span></span></p></td><td><p><span><span>100</span></span></p></td></tr><tr><td></td><td><p><span><span>MIN of C</span></span></p></td><td><p><span><span>12</span></span></p></td><td><p><span><span>1</span></span></p></td></tr><tr><td><p><span><span>2/4</span></span></p></td><td><p><span><span>MAX of A</span></span></p></td><td><p><span><span>100</span></span></p></td><td><p><span><span>100</span></span></p></td></tr><tr><td></td><td><p><span><span>MIN of C</span></span></p></td><td><p><span><span>14</span></span></p></td><td><p><span><span>19</span></span></p></td></tr><tr><td><p><span><span>2/5</span></span></p></td><td><p><span><span>MAX of A</span></span></p></td><td><p><span><span>450</span></span></p></td><td></td></tr><tr><td></td><td><p><span><span>MIN of C</span></span></p></td><td><p><span><span>9</span></span></p></td><td></td></tr></tbody></table>

   ```
   2/5 and Down
   ```
5. In the following SQL query, which column is part of an addition operation that creates a new column?
   ```
   SELECT Yes_Responses, No_Responses, Total_Surveys, Yes_Responses + No_Responses AS Responses_Per_Survey FROM Survey_1
   ```
   ```
   Yes_Responses
   ```
6. What SQL operator is used to return the remainder of a division operation?
   ```
   %
   ```
7. What is the process of checking and rechecking the quality of your data so that it is complete, accurate, secure, and consistent?
   ```
   Data validation
   ```
8. What is the purpose of the != operator in SQL?
   ```
   To check if two values or expressions are not equal
   ```
9. What is a reason to use a temporary table instead of a standard table in SQL?
   ```
   A temporary table calculates formulas using less memory than standard tables.
   ```
10. Which of the following SQL queries adds a table into the database? Select all that apply.

    ```
    • CREATE TABLE my_table AS (SELECT * FROM other_table);
    • WITH my_table AS (SELECT * FROM other_table WHERE x = 0);
    ```