## Course challenge
1. **Scenario 1, questions 1-5**
   <br/><br/>
   You are a data analyst at a small analytics company. Your company is hosting a project kick-off meeting with a new client, Meer-Kitty Interior Design. The agenda includes reviewing their goals for the year, answering any questions, and discussing their available data.
   <br/><br/>
   Before the meeting you review the About Us tab on their website and their business plan, linked below:
   <br/><br/>
   [Meer-Kitty-Interior-Design-About-Us-Page.pdf](supplementary-materials/course-challenge-Meer-Kitty-Interior-Design-About-Us-Page.pdf)

   [Meer-Kitty-Interior-Design-Business-Plan.pdf](supplementary-materials/course-challenge-Meer-Kitty-Interior-Design-Business-Plan.pdf)
   <br/><br/>
   Meer-Kitty Interior Design has two goals. They want to expand their online audience, which means getting their company and brand known by as many people as possible. They also want to launch a line of high-quality indoor paint to be sold in-store and online. You decide to consider the data about indoor paint first.
   <br/><br/>
   [Kitty-Survey-Feedback.csv](supplementary-materials/course-challenge-Kitty-Survey-Feedback.csv)
   <br/><br/>
   When you refer to the **Meer-Kitty survey feedback** tab, you are pleased to find that the available data is aligned to the business objective. However, you do some research about confidence level for this type of survey and learn that you need at least 120 unique responses for the survey results to be useful. Therefore, the dataset has two limitations: First, there are only 40 responses; second, a Meer-Kitty superfan, User 588, completed the survey 11 times.
   <br/><br/>
   **As the survey has too few responses and numerous duplicates that are skewing results, you decide to repeat the survey in order to create a new, improved dataset. What is your first step?**
   ```   
   Talk with stakeholders, explain the new timeline, and ask for approval.
   ```
2. **Scenario 1 continued**
   <br/><br/>
   During the meeting, you also learn that Meer-Kitty videos are hosted on their website. For each product offered, there is an accompanying video for customers to learn more. So, more views for a video suggests greater consumer interest.
   <br/><br/>
   Your goal is to identify which videos are most popular, so Meer-Kitty knows what topics to explore in the future. Unfortunately, Meer-Kitty has just three months of data available because they only recently launched the videos on their site.
   <br/><br/>
   **Without enough data to identify long-term trends about the video subjects that people prefer, what are your available options? Select all that apply.**
   ```
   Ask to wait for more data and provide Meer-Kitty with an updated timeline.
   Talk with Meer-Kitty stakeholders and ask to adjust the objective.
   ```
3. **Scenario 1 continued**
   <br/><br/>
   Now that you’ve identified some limitations with Meer-Kitty’s data, you want to communicate your concerns to stakeholders. In addition to insufficient video trend data, your main concern with the indoor paint survey is that the data isn’t representative of the population as a whole.
   <br/><br/>
   **Clearly, one particular respondent, the superfan, is overrepresented. What does this situation describe?**
   ```
   Sampling bias
   ```
4. **Scenario 1 continued**
   <br/><br/>
   The stakeholders understand your concerns and agree to repeat the indoor paint survey. In a few weeks, you have a much better dataset with more than 150 responses and no duplicates.
   <br/><br/>
   To use the template for the survey feedback, click the link below and select “Use Template.”
   <br/><br/>
   [New-Kitty-Survey-Feedback.csv](supplementary-materials/course-challenge-New-Kitty-Survey-Feedback.csv)
   <br/><br/>
   If you are using the template, please refer to the **New Meer-Kitty survey feedback** tab _located at the bottom of the page_. You notice that questions 4 and 5 are dependent on the respondent’s answer to question 3. So, you need to determine how many people answered Yes to question 3, then compare that to responses to questions 4 and 5. That way, you will know if questions 4 and 5 have any nulls.
   <br/><br/>
   **You decide to use a spreadsheet tool that changes how cells appear when they contain the word Yes. When using this tool, what is the word Yes?**
   ```
   The value in a conditional formatting rule
   ```
5. **Scenario 1, continued**
   <br/><br/>
   You continue cleaning the data. You use tools such as remove duplicates and COUNTIF to ensure the dataset is complete, correct, and relevant to the problem you’re trying to solve. Then, you complete the verification and reporting processes to share the details of your data-cleaning effort with your team.
   <br/><br/>
   While reviewing, your team notes one aspect of data cleaning that would improve the dataset even more. They point out that the new survey also has a new question in Column G: “What are your favorite indoor paint colors?” This was a free-response question, so respondents typed in their answers. Some people included multiple different colors of paint. In order to determine which colors are most popular, it will be necessary to put each color in its own cell.
   <br/><br/>
   **What spreadsheet function enables you to put each of the colors in Column G into a new, separate cell?**
   ```
   SPLIT
   ```
6. **Scenario 2, questions 6-10**
   <br/><br/>
   You’ve completed this program and are interviewing for a junior data scientist position. The job is at B.Spoke Market Research, a company that analyzes market conditions using customer surveys and other research methods. The detailed job description can be found below:
   <br/><br/>
   [Spoke-Market-Research-Job-Description.pdf](supplementary-materials/course-challenge-Spoke-Market-Research-Job-Description.pdf)
   <br/><br/>
   So far, you’ve had a phone interview with a recruiter and you’ve secured a second interview with the B.Spoke team. The recruiter’s email can be found below:
   <br/><br/>
   [course-challenge-Email-from-Recruiter.pdf](supplementary-materials/course-challenge-Email-from-Recruiter.pdf)
   <br/><br/>
   You arrive 15 minutes early for your interview. Soon, you are escorted into a conference room, where you meet Jodie Choi, the data science lead. After welcoming you, the behavioral interview begins.
   <br/><br/>
   For your first question, your interviewer wants to learn about your experience with spreadsheets. She says: Sometimes the team needs data that is stored in different spreadsheets. So, we use a spreadsheet function to find the information we need.
   <br/><br/>
   **There is a spreadsheet function that searches for a value in the first column of a given range and returns the value of a specified cell in the row in which it is found. It is called SEARCH.**
   ```
   Felse
   ```
7. **Scenario 2, continued**
   <br/><br/>
   Next, your interviewer wants to know more about your understanding of tools that work in both spreadsheets and SQL queries. She explains that the data her team receives from customer surveys sometimes has many duplicate entries.
   <br/><br/>
   **She says: Spreadsheets have a great tool for that called remove duplicates. But when writing a SQL query, what command should you include in your SELECT statement to remove duplicates?**
   ```
   DISTINCT
   ```
8. Scenario 2, continued
   <br/><br/>
   Now, your interviewer explains that the data team usually works with very large amounts of customer survey data. After receiving the data, they import it into a SQL table. But sometimes, the new dataset imports incorrectly and they need to change the format.
   <br/><br/>
   **She asks: What function would you use to convert data in a SQL table from one datatype to another?**
   ```
   CAST
   ``` 
9. **Scenario 2, continued**
   <br/><br/>
   Next, your interviewer explains that one of their clients is an online retailer that needs to create product numbers for a vast inventory. Her team does this by combining the text strings for product number, manufacturing date, and color.
   <br/><br/>
   **She asks: If you encountered a situation where you wanted to add strings together to create new text strings, which SQL function would you use?**
   ```
   CONCAT
   ```
10. **Scenario 2, continued**
   <br/><br/>
   For your final question, your interviewer explains that her team often comes across data with extra leading or trailing spaces.
   <br/><br/>
   **She asks: Which SQL function enables you to eliminate those extra spaces for consistency?**
   ```
   TRIM
   ```