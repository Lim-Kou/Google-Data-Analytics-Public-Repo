## Weekly challenge 3
1. In data analytics, what is the process of gathering data from multiple sources and combining it into a single, summarized collection?
   ```
   Data aggregation
   ```
2. A data analyst uses the TRIM function on their spreadsheet. Why might they do this?
   ```
   They plan to use VLOOKUP on the spreadsheet data.
   ```
3. When using VLOOKUP, there are some common limitations that data analysts should be aware of. Identify these limitations. Select all that apply.
   ```
   • VLOOKUP can only return a value from the data to the right of the column of the matched value.
   • VLOOKUP only returns the first match it finds, even if there are many possible matches.
   ```
4. A data analyst wraps the data array for their function in dollar signs ($). What does this do? Select all that apply.
   ```
   • It creates an absolute reference.
   • It makes it so that columns cannot be changed.
   • It makes it so that rows cannot be changed.
   ```
5. The following is a selection from a spreadsheet:
   <table><tbody><tr><td><p><span><span>N/A</span></span></p></td><td><p><span><span>A</span></span></p></td><td><p><span><span>B</span></span></p></td><td><p><span><span>C</span></span></p></td></tr><tr><td><p><span><span>1</span></span></p></td><td><p><span><strong><span>Country</span></strong></span></p></td><td><p><span><strong><span>Population in 2020</span></strong></span></p></td><td><p><span><strong><span>Growth in population 2000-2020</span></strong></span></p></td></tr><tr><td><p><span><span>2</span></span></p></td><td><p><span><span>China</span></span></p></td><td><p><span><span>1,439,323,776</span></span></p></td><td><p><span><span>13.4 %</span></span></p></td></tr><tr><td><p><span><span>3</span></span></p></td><td><p><span><span>India</span></span></p></td><td><p><span><span>1,380,004,385</span></span></p></td><td><p><span><span>37.1 %</span></span></p></td></tr><tr><td><p><span><span>4</span></span></p></td><td><p><span><span>United States</span></span></p></td><td><p><span><span>331,002,651</span></span></p></td><td><p><span><span>17.3 %</span></span></p></td></tr><tr><td><p><span><span>5</span></span></p></td><td><p><span><span>Indonesia</span></span></p></td><td><p><span><span>273,523,615</span></span></p></td><td><p><span><span>27.7%</span></span></p></td></tr><tr><td><p><span><span>6</span></span></p></td><td><p><span><span>Pakistan</span></span></p></td><td><p><span><span>220,892,340</span></span></p></td><td><p><span><span>44.9%</span></span></p></td></tr><tr><td><p><span><span>7</span></span></p></td><td><p><span><span>Brazil</span></span></p></td><td><p><span><span>212,559,417</span></span></p></td><td><p><span><span>21.9%</span></span></p></td></tr><tr><td><p><span><span>8</span></span></p></td><td><p><span><span>Nigeria</span></span></p></td><td><p><span><span>206,139,589</span></span></p></td><td><p><span><span>66.3%</span></span></p></td></tr><tr><td><p><span><span>9</span></span></p></td><td><p><span><span>Bangladesh</span></span></p></td><td><p><span><span>164,689,383</span></span></p></td><td><p><span><span>27.9%</span></span></p></td></tr><tr><td><p><span><span>10</span></span></p></td><td><p><span><span>Russia</span></span></p></td><td><p><span><span>145,934,462</span></span></p></td><td><p><span><span>-0.8%</span></span></p></td></tr></tbody></table>

   To search for the population of Pakistan, what is the correct VLOOKUP syntax?
   ```
   =VLOOKUP("Pakistan", A2:B10, 2, false)
   ```
6. A data analyst writes a query in SQL with the RIGHT JOIN function
   ```
   FROM fiction_table 
   RIGHT JOIN books_table
   ```
7. What does this function do?
   ```
   It returns all records in the books table and only the records from the fiction table with matching values.
   ```
8. The COUNT DISTINCT function includes repeating values when returning values in a specified range.
   ```
   False
   ```
9. Which of the following terms describe a subquery? Select all that apply.
   ```
   • Inner select
   • Nested query
   • Inner query 
   ```