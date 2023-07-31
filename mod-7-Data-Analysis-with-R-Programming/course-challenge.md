## Course challenge
1. **Scenario 1, questions 1-7**
   As part of the data science team at Gourmet Analytics, you use data analytics to advise companies in the food industry. You clean, organize, and visualize data to arrive at insights that will benefit your clients. As a member of a collaborative team, sharing your analysis with others is an important part of your job.
   <br/><br/>
   Your current client is Chocolate and Tea, an up-and-coming chain of cafes.
   <br/><br/>
   The eatery combines an extensive menu of fine teas with chocolate bars from around the world. Their diverse selection includes everything from plantain milk chocolate, to tangerine white chocolate, to dark chocolate with pistachio and fig. The encyclopedic list of chocolate bars is the basis of Chocolate and Tea’s brand appeal. Chocolate bar sales are the main driver of revenue.
   <br/><br/>
   Chocolate and Tea aims to serve chocolate bars that are highly rated by professional critics. They also continually adjust the menu to make sure it reflects the global diversity of chocolate production. The management team regularly updates the chocolate bar list in order to align with the latest ratings and to ensure that the list contains bars from a variety of countries.
   <br/><br/>
   They’ve asked you to collect and analyze data on the latest chocolate ratings. In particular, they’d like to know which countries produce the highest-rated bars of super dark chocolate (a high percentage of cocoa). This data will help them create their next chocolate bar menu.
   <br/><br/>
   Your team has received a dataset that features the latest ratings for thousands of chocolates from around the world. Click [here](https://www.kaggle.com/rtatman/chocolate-bar-ratings "Hyperlink to dataset") to access the dataset. Given the data and the nature of the work you will do for your client, your team agrees to use R for this project.
   <br/><br/>
   **A teammate asks you about the benefits of using R for the project. You mention that R can quickly process lots of data and create high quality data visualizations. What is another benefit of using R for the project?**
   ```
   Easily reproduce and share an analysis
   ```
2. **Scenario 1, continued**
   <br/><br/>
   Before you begin working with your data, you need to import it and save it as a data frame. To get started, you open your RStudio workspace and load the tidyverse library. You upload a .csv file containing the data to RStudio and store it in a project folder named flavors_of_cacao.csv.
   <br/><br/>
   **You use the read_csv() function to import the data from the .csv file. Assume that the name of the data frame is chocolate_df and the .csv file is in the working directory.** **What code chunk lets you create the data frame?**
   ```
   chocolate_df <-read_csv("flavors_of_cacao.csv")
   ```
3. **Scenario 1, continued**
   <br/><br/>
   Now that you’ve created a data frame, you want to find out more about how the data is organized. The data frame has hundreds of rows and lots of columns.
   <br/><br/>
   **Assume the name of your data frame is flavors_df.** **What code chunk lets you review the structure of the data frame?**
   ```
   str(flavors_df)
   ```
4. **Scenario 1, continued**
   <br/><br/>
   Next, you begin to clean your data. When you check out the column headings in your data frame you notice that the first column is named _Company...Maker.if.known._ (Note: The period after _known_ is part of the variable name.) For the sake of clarity and consistency, you decide to rename this column _Company_ (without a period at the end).
   <br/><br/>
   **Assume the first part of your code chunk is:**
   <br/><br/>
   ```flavors_df %>%```
   <br/><br/>
   **What code chunk do you add to change the column name?**
   ```
   (Company = Company...Maker.if.known.)
   ```
5. After previewing and cleaning your data, you determine what variables are most relevant to your analysis. Your main focus is on _Rating_, _Cocoa.Percent_, and _Company.Location_. You decide to use the select() function to create a new data frame with only these three variables.
   <br/><br/>
   **Assume the first part of your code is:** 
   <br/><br/>
   ```trimmed_flavors_df <- flavors_df %>%```
   <br/><br/>
   **Add the code chunk that lets you select the three variables.**
   <br/><br/>
   ```select(Rating, Cocoa.Percent, Company.Location)```
   <br/><br/>
   What company location appears in row 1 of your tibble?
   ```
   France
   ```
6. Next, you select the basic statistics that can help your team better understand the ratings system in your data. 
   <br/><br/>
   **Assume the first part of your code is:**
   <br/><br/>
   trimmed_flavors_df %>%
   <br/><br/>
   **You want to use the summarize() and sd() functions to find the standard deviation of the rating for your data. Add the code chunk that lets you find the standard deviation for the variable** _**Rating.**_
   <br/><br/>
   ```summarise(sd(Rating))```
   <br/><br/>
   What is the standard deviation of the rating?
   ```
   0.4780624
   ```
7. After completing your analysis of the rating system, you determine that any rating greater than or equal to 3.9 points can be considered a high rating. You also know that Chocolate and Tea considers a bar to be super dark chocolate if the bar's cocoa percent is greater than or equal to 75%. You decide to create a new data frame to find out which chocolate bars meet these two conditions.
   <br/><br/>
   **Assume the first part of your code is:**
   <br/><br/>
   ```best_trimmed_flavors_df <- trimmed_flavors_df %>% ```
   <br/><br/>
   **You want to apply the filter() function to the variables** _**Cocoa.Percent**_ **and** _**Rating**_**. Add the code chunk that lets you filter the data frame for chocolate bars that contain at least 75% cocoa and have a rating of at least 3.9 points.**
   <br/><br/>
   ```filter(Cocoa.Percent >= "75%" & Rating >= 3.9)```
   <br/><br/>
   What value for cocoa percent appears in row 1 of your tibble?
   ```
   75%
   ```
8. Now that you’ve cleaned and organized your data, you’re ready to create some useful data visualizations. Your team assigns you the task of creating a series of visualizations based on requests from the Chocolate and Tea management team. You decide to use ggplot2 to create your visuals. 
   <br/><br/>
   **Assume your first line of code is:**
   <br/><br/>
   ```ggplot(data = best_trimmed_flavors_df) +```
   <br/><br/>
   **You want to use the geom_bar() function to create a bar chart. Add the code chunk that lets you create a bar chart with the variable** _**Company.Location**_ **on the x-axis.**
   <br/><br/>
   ```geom_bar(aes(x=Company.Location))```
   <br/><br/>
   How many bars does your bar chart display?
   ```
   5
   ```
9. Your bar chart reveals the locations that produce the highest rated chocolate bars. To get a better idea of the specific rating for each location, you’d like to highlight each bar.
   <br/><br/>
   **Assume that you are working with the code chunk:**
   <br/><br/>
   ```ggplot(data = best_trimmed_flavors_df) +```
   ```  geom_bar(mapping = aes(x = Company.Location))```
   <br/><br/>
   **Add a code chunk to the second line of code to map the aesthetic** _**color**_ **to the variable** _**Rating**_**.**
   <br/><br/>
   **NOTE: the three dots (...) indicate where to add the code chunk.**
   <br/><br/>
   ```geom_bar(mapping = aes(x = Company.Location, color = Rating))```
   <br/><br/>
   **According to your bar chart, which two company locations produce the highest rated chocolate bars?**
   ```
   Canada and France
   ```
10. **Scenario 2, continued**
    <br/><br/>
    A teammate creates a new plot based on the chocolate bar data. The teammate asks you to make some revisions to their code.
    <br/><br/>
    **Assume your teammate shares the following code chunk:**
    <br/><br/>
    ```ggplot(data = best_trimmed_flavors_df) +```
    ```geom_bar(mapping = aes(x = Company)) +```
    <br/><br/>
    **What code chunk do you add to the third line to create wrap around facets of the variable** _**Company**_**?**
    ```
    facet_wrap(~Company)
    ```
11. **Scenario 2, continued**
    <br/><br/>
    Your team has created some basic visualizations to explore different aspects of the chocolate bar data. You’ve volunteered to add titles to the plots. You begin with a scatterplot.
    <br/><br/>
    **Assume the first part of your code chunk is:**
    <br/><br/>
    ```ggplot(data = trimmed_flavors_df) +```
    ```geom_point(mapping = aes(x = Cocoa.Percent, y = Rating)) +```
    <br/><br/>
    **What code chunk do you add to the third line to add the title** _**Best Chocolates**_ **to your plot?**
    ```
    labs(title = “Best Chocolates”)
    ```
12. **Scenario 2, continued**
    <br/><br/>
    Next, you create a new scatterplot to explore the relationship between different variables. You want to save your plot so you can access it later on. You know that the ggsave() function defaults to saving the last plot that you displayed in RStudio, so you’re ready to write the code to save your scatterplot.  
    <br/><br/>
    **Assume your first two lines of code are:**
    <br/><br/>
    ```ggplot(data = trimmed_flavors_df) +```
    `````  geom_point(mapping = aes(x = Cocoa.Percent, y = Rating)) +`````
    <br/><br/>
    **What code chunk do you add to the third line to save your plot as a pdf file with “chocolate” as the file name?**
    ```
    ggsave(“chocolate.pdf”)
    ```

13. **Scenario 2, continued**
    <br/><br/>
    As a final step in the analysis process, you create a report to document and share your work. Before you share your work with the management team at Chocolate and Tea, you are going to meet with your team and get feedback. Your team wants the documentation to include all your code and display all your visualizations.
    <br/><br/>
    **You decide to create an R Markdown notebook to document your work. What are your reasons for choosing an R Markdown notebook? Select all that apply.**
    ```
    • It displays your data visualizations
    • It lets you record and share every step of your analysis
    • It allows users to run your code
    ```

