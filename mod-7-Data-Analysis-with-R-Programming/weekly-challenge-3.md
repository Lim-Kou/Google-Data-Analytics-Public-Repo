## Weekly challenge 3
1. A data analyst creates a data frame with data that has more than 50,000 observations in it. When they print their data frame, it slows down their console. To avoid this, they decide to switch to a tibble. Why would a tibble be more useful in this situation?
   ```
   Tibbles won’t overload the console because they automatically only print the first 10 rows of data and as many variables as will fit on the screen
   ```
2. A data analyst is working with a large data frame. It contains so many columns that they don’t all fit on the screen at once. The analyst wants a quick list of all of the column names to get a better idea of what is in their data. What function should they use?
   ```
   colnames()
   ```
3. You are working with the ToothGrowth dataset. You want to use the skim_without_charts() function to get a comprehensive view of the dataset. Write the code chunk that will give you this view.
   ```
   skim_without_charts(ToothGrowth)
   ```
   ```
   18.8
   ```
4. A data analyst is working with the penguins dataset. What code chunk does the analyst write to make sure all the column names are unique and consistent and contain only letters, numbers, and underscores?
   ```
   clean_names(penguins)
   ```
5. A data analyst is working with the penguins data. The analyst wants to sort the data by _flipper_length_m_ from longest to shortest. What code chunk will allow them to sort the data in the desired order?
   ```
   penguins %>% arrange(-flipper_length_mm)
   ```
6. You are working with the penguins dataset. You want to use the summarize() and min() functions to find the minimum value for the variable _bill_depth_mm._ At this point, the following code has already been written into the script:
   ```
   penguins %>%
   drop_na() %>%
   group_by(species) %>%
   ```
   Add the code chunk that lets you find the minimum value for the variable _bill_depth_mm._
   ```
   summarize(min(bill_depth_mm))
   ```
   What is the minimum bill depth in mm for the Chinstrap species?
   ```
   16.4
   ```
7. A data analyst is working with a data frame called _zoo_records_. They want to create a new column named _is_large_animal_ that signifies if an animal has a weight of more than 199 kilograms. What code chunk lets the analyst create the _is_large_animal_ column?
   ```
   zoo_records %>% mutate(is_large_animal = weight > 199)
   ```
8. A data analyst is working with a data frame named _customers_. It has separate columns for area code (_area_code_) and phone number (_phone_num_). The analyst wants to combine the two columns into a single column called _phone_number_, with the area code and phone number separated by a hyphen. What code chunk lets the analyst create the _phone_number_column?
   ```
   unite(customers, “phone_number”, area_code, phone_num, sep=”-”)
   ```
9. In R, which statistical measure can help you understand the spread of values in a dataset and describe how far each value is from the mean?
   ```
   Standard deviation
   ```
10. A data analyst creates two different predictive models for the same dataset. They use the bias() function on both models. The first model has a bias of 20. The second model has a bias of 0.1. Which model is less biased?
    ```
    The second model
    ```