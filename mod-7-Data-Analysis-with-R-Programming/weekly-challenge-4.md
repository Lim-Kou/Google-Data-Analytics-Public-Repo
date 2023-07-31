## Weekly challenge 4
1. Which of the following are benefits of using ggplot2? Select all that apply.
   ```
   • Easily adds layers to your plot
   • Combines data manipulation and visualization
   • Customizes the look and feel of your plot
   ```
2. A data analyst creates a bar chart with the diamonds dataset. They begin with the following line of code:
   ```
   ggplot(data = diamonds)
   ```
   What symbol should the analyst put at the end of the line of code to add a layer to the plot?
   ```
   The plus sign (+)
   ```
3. A data analyst creates a plot using the following code chunk:
   ```
   ggplot(data = buildings) +
   geom_bar(mapping = aes(x = construction_year, color = height))
   ```
   Which of the following represents an aesthetic attribute in the code chunk?
   ```
   x
   ```
4. Fill in the blank: In ggplot2, the term mapping refers to the connection between variables and _____ .
   ```
   aesthetics 
   ```
5. A data analyst is working with the following plot and gets an error caused by a bug. What is the cause of the bug?
   ```
   ggplot(data = penguins)
   + geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g))
   ```
   ```
   The plus should be at the end of the first line.
   ```
6. You are working with the penguins dataset. You create a scatterplot with the following code chunk: 
   ```
   ggplot(data = penguins) +
   geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g))
   ```
   You want to highlight the different penguin species in your plot. Add a code chunk to the second line of code to map the aesthetic _size_ to the variable _bill_depth_mm_.
   <br/><br/>
   NOTE: the three dots (...) indicate where to add the code chunk. You may need to scroll in order to find the dots.
   ```
   geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g, size = bill_depth_mm))
   ```
   Which approximate range of bill depths does your visualization display?
   ```
   14 - 20
   ```
7. Which aesthetic of the geom_smooth function can be used to change the style of the line?
   ```
   linetype
   ```
8. You are working with the diamonds dataset. You create a bar chart with the following code: 
   ```
   ggplot(data = diamonds) +
   geom_bar(mapping = aes(x = color, fill = cut)) +
   ```
   You want to use the facet_wrap() function to display subsets of your data. Add the code chunk that lets you facet your plot based on the variable _cut._
   ```
   facet_wrap(~cut)
   ```
   How many subplots does your visualization show?
   ```
   5
   ```
9. A data analyst uses the annotate() function to create a text label for a plot. Which attributes of the text can the analyst change by adding code to the argument of the annotate() function? Select all that apply.
   ```
   • Change the color of the text.
   • Change the size of the text.
   • Change the font style of the text.
   ```
10. Which statement about the ggsave() function is correct?
    ```
    ggsave() exports the last plot displayed by default.
    ```