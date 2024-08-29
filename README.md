# Data-cleaning- Life Expectancy data

## Dataset description
The Global Health Observatory (GHO) data repository under World Health Organization (WHO) keeps track of the health status as well as many other related factors for all countries The data-sets are made available to public for the purpose of health data analysis. The data-set related to life expectancy, health factors for 193 countries has been collected from the same WHO data repository website and its corresponding economic data was collected from United Nation website. Among all categories of health-related factors only those critical factors were chosen which are more representative. It has been observed that in the past 15 years , there has been a huge development in health sector resulting in improvement of human mortality rates especially in the developing nations in comparison to the past 30 years. Therefore, in this project we have considered data from year 2000-2015 for 193 countries for further analysis. The individual data files have been merged together into a single data-set. On initial visual inspection of the data showed some missing values. As the data-sets were from WHO, we found no evident errors. Missing data was handled in R software by using Missmap command. The result indicated that most of the missing data was for population, Hepatitis B and GDP. The missing data were from less known countries like Vanuatu, Tonga, Togo, Cabo Verde etc. Finding all data for these countries was difficult and hence, it was decided that we exclude these countries from the final model data-set. The final merged file(final dataset) consists of 22 Columns and 2938 rows which meant 20 predicting variables.

## Data preprocessing
1. Importing Libraries : Brings in tools (like pandas, numpy, seaborn, etc.) that help you handle data, create visuals, and build models.

2. Loading the Data: Reads the life expectancy data from a file and shows a preview of the first and last few rows, as well as the number of rows and columns.

3. Checking the Data: Looks at the data’s structure, such as the types of data in each column, and identifies any missing values.

4. Handling Missing Data: Finds and fills in missing numbers using a method that looks at similar data points nearby (KNNImputer).

5. Removing Duplicate Entries: Checks if there are any exact duplicate rows and removes them to keep only unique data.

6. Visualizing the Data: Creates different types of charts:
Boxplots: To find any extreme values (outliers) in the data.
Histograms: To see how data is spread out.
Scatterplots: To explore the relationship between two pieces of data.

7. Handling Outliers: Identifies and adjusts extreme values in certain columns to prevent them from skewing results.

8. Saving the Cleaned Data: Saves the cleaned-up data to a new file for future use.

9. Analyzing Life Expectancy Trends: Creates simple charts to explore key insights, such as:
The difference in life expectancy between developed and developing countries.
How life expectancy has changed over time.
The relationship between population size and life expectancy.

10. Preparing for Machine Learning: Prepares the data for building a predictive model by:
Converting categorical data (like country names) into numbers.
Splitting the data into a training set (to learn from) and a test set (to evaluate the model).

11. Building a Linear Regression Model: Creates a model to predict life expectancy based on other factors.
Checks how well the model works by comparing predicted values with actual values.
Shows how close the predictions are to real life using error measures.

12. Visualizing Model Results: Plots the predicted life expectancy against the actual values to see how accurate the model is.
This process helps in cleaning the data, understanding it through visualization, and then building a model to make predictions.
