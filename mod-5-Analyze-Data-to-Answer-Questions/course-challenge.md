## Course challenge
1. **Scenario 1, Questions 1-7**
   <br /><br />
   For the past six months, you have been working for a direct-mail marketing firm as a junior marketing analyst. Direct mail is advertising material sent to people through the mail. These people can be current or prospective customers, clients, or donors. Many charities depend on direct mail for financial support.
   <br /><br />
   Your company, Directly Dynamic, creates direct-mail pieces with its in-house staff of graphic designers, expert mail list services, and on-site printing. Your team has just been hired by a local nonprofit, Food Justice Rock Springs. The mission of Food Justice Rock Springs is to eliminate food deserts by establishing local gardens, providing mobile pantries, educating residents, and more. Click below to read the email from Tayen Bell, vice president of marketing and outreach.
    <br /><br />
   [Course-Challenge-Email-From-Tayen-Bell-Directly-Dynamic.pdf](supplementary-materials/Course-Challenge-Email-From-Tayen-Bell-Directly-Dynamic.pdf)
   <br /><br />
   You begin by reviewing the dataset. To use the template for this dataset, click the link below and select “Use Template.”
   <br /><br />
   [Course-Challenge-Dynamic-Dataset.xlsx](supplementary-materials/Course-Challenge-Dynamic-Dataset.xlsx)
   <br /><br />
   The client has asked you to send two separate mailings: one to people within 50 miles of Rock Springs; the other to anyone outside that area. So, to research each donor’s distance from the city, you first need to find out where all of these people live.
   <br /><br />
   You could scroll through 209 rows of data, but you know there is a more efficient way to organize the cities.
   <br /><br />
   **Which of the following procedures will enable you to sort your spreadsheet by city (Column K) in ascending order? Select all that apply.**
   ```
   • Select A2-R210, then use the drop-down menu to Sort Sheet by Column K from A to Z
   • Use the SORT function syntax: =SORT(A2:R210, 11, TRUE)
   ```
2. **Scenario 1, continued**
   <br /><br />
   You notice that many cells in the city column, Column K, are missing a value. So, you use the zip codes to research the correct cities. Now, you want to add the cities to each donor’s row. However, you are concerned about making a mistake, such as a spelling typo.
   <br /><br />
   **What spreadsheet tool allows you to control what can and cannot be entered in your worksheet in order to avoid typos?**
   ```
   Data validation
   ```
3. **Scenario 1, continued**
   <br /><br />
   Now, you decide to address Tayen’s request to include a handwritten note in the direct-mail piece for anyone who gave at least $100 last year.
   <br /><br />
   **Which of the following procedures will enable you to change how cells in your spreadsheet appear if they contain a value of $100 or more?**
   ```
   Select Column M. Then, select Format > Conditional Formatting. Choose to format cells if they are greater than or equal to 100.
   ```
4. **Scenario 1, continued**
   <br /><br />
   At this point, you notice that the information about state and zip code is in the same cell. However, your company’s mailing list software requires states to be on a separate line from zip codes.
   <br /><br />
   **To move the 5-digit zip code in cell L2 into its own column, you use the function =LEFT(L2,5).**
   ```
   False
   ```
5. **Scenario 1, continued**
   <br /><br />
   Next, you duplicate your dataset twice using the Sheet Menu. You rename the first sheet Donation Form List, and you remove the cities that are further than 50 miles from Rock Springs. You rename the second sheet Postcard List, and you remove the cities that are within 50 miles of Rock Springs.
   <br /><br />
   Then, you import these datasets into your company’s mailing list database. In a mailing list database, you create two tables: Donation_Form_List and Postcard_List. You decide to clean the Donation_Form_List first.
   <br /><br />
   Your company’s mailing list software requires units to be on the same line as street addresses. However, they are currently in two separate columns (street_address and unit).
   <br /><br />
   **What portion of your SQL statement will instruct the database to combine these two columns into a new column called “address”?**
   ```
   CONCAT(street_address, " to ", unit) AS address
   ```
6. **Scenario 1, continued**
   <br /><br />
   Your database contains people who live in many areas of Wyoming. However, it’s important to align your in-house data with the data from Food Justice Rock Springs. You also need to separate your data into the two lists: Donation_Form_List and Postcard_List. They will be based on each city’s distance from Rock Springs.
   <br /><br />
   **The zip codes are in a column called zip_code. To select all data from the Donation_Form_List organized by zip code, you use the ORDER BY function. The syntax is:**
   ```
   SELECT *
   FROM Donation_Form_List
   ORDER BY zip_code
   ```
   ``` 
   True
   ```
7. **Scenario 1, continued**
   <br /><br />
   You finish cleaning your datasets, so you decide to review Tayen’s email one more time to make sure you completed the task fully. It’s a good thing you checked because you forgot to identify people who have served on the board of directors or board of trustees. She wants to write them a thank-you note, so you need to locate them in the database.
   <br /><br />
   **To retrieve only those records that include people who have served on the board of trustees or on the board of directors, what clause do you include in your query?**
   ```
   WHERE Board_Member = "TRUE" OR Trustee = "TRUE"
   ```
8. **Scenario 2, Questions 8-13**
   <br /><br />
   Your company’s direct-mail campaign was very successful, and Food Justice Rock Springs has continued partnering with Directly Dynamic. One thing you’ve been working on is assigning all donors identification numbers. This will enable you to clean and organize the lists more effectively.
   <br /><br />
   Meanwhile, another team member has been creating a prospect list that contains data about people who have indicated interest in getting involved with Food Justice Rock Springs. These people are also assigned a unique ID. Now, you need to compare your donor list with the dataset in your database and collect certain data from both.
   <br /><br />
   **What SQL function will return records with matching values in both tables?**
   ```
   INNER JOIN 
   ```
9. **Scenario 2, continued**
   <br /><br />
   Your next task is to identify the average contribution given by donors over the past two years. Tayen will use this information to set a donation minimum for inviting donors to an upcoming event.
   <br /><br />
   **You start with 2019. To return average contributions in 2019 (contributions_2019), you use the AVG function. What section of a SQL query will instruct the database to find this average and store it in the AvgLineTotal variable?**
   ```
   AVG(contributions_2019) AS AvgLineTotal
   ```
10. **Scenario 2, continued**
    <br /><br />
    Now that you provided her with the average donation amount, Tayen decides to invite 50 people to the grand opening of a new community garden. You return to your New Donor List spreadsheet to determine how much each donor gave in the past two years. You will use that information to identify the 50 top donors and invite them to the event.
    <br /><br />
    **What is the correct syntax to add the contribution amounts in cells O2 and P2?**
    ```
    =SUM(O2,P2)
    ```
11. **Scenario 2, continued**
    <br /><br />
    Tayen informs you that she’s thinking about inviting anyone who donated at least $100 in 2018, as well. However, she only has five open spaces. She asks you to report how many people gave at least $100 so she can determine if they can also be invited to the event.
    <br /><br />
    **What is the correct syntax to count how many donations of $100 or greater appear in Column O (Contributions 2018)?**
    ```
    =COUNTIF(O2:O210,">=100")
    ```
12. **Scenario 2, continued**
    <br /><br />
    The community garden grand opening was a success. In addition to the 55 donors Food Justice Rock Springs invited, 20 other prospects attended the event. Now, Tayen wants to know more about the donations that came in from new prospects compared to the original donors.
    <br /><br />
    **This SQL query can be used to identify the percentage of contributions from prospects compared to total donors:**
    ```
    SELECT 
    event_contributions,
    Total_donors,
    Total_prospects,
    (Total_prospects / Total_donors * 100) AS Prospects_Percent
    FROM contributions_data 
    ```
    ```
    True
    ```
13. **Scenario 2, continued**
    <br /><br />
    Your team creates a highly effective prospects list for Food Justice Rock Springs. After a few months, many of these prospects become donors. Now, Tayen wants to know the top three cities in which these new donors live. She will use that information to determine if it’s still true that people who live closer to Rock Springs are more likely to donate.
    <br /><br />
    **Which SQL query will retrieve the number of donors in each city, sorted high to low?**
    ```
    SELECT COUNT(DonorID), City
    FROM new_donor_list
    GROUP BY City
    ORDER BY COUNT(DonorID) DESC
    ```