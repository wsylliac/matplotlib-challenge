# matplotlib-challenge
# Module 5 Challenge

What good is data without a good plot to tell the story?
In this assignment, you’ll apply what you've learned about Matplotlib to a real-world situation and dataset.

## Background

You've just joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.

## Files

Download the following files to help you get started:

[Module 5 Challenge Files](https://static.bc-edx.com/data/dl-1-2/m5/lms/starter/Starter_Code.zip) 📁

## Instructions

This assignment is broken down into the following tasks:

* Prepare the data.
* Generate summary statistics.
* Create bar charts and pie charts.
* Calculate quartiles, find outliers, and create a box plot.
* Create a line plot and a scatter plot.
* Calculate correlation and regression.
* Submit your final analysis.


## Prepare the Data
1. Run the provided package dependency and data imports, and then merge the <img width="118" alt="Screenshot 2023-10-17 at 1 49 50 PM" src="https://github.com/wsylliac/matplotlib-challenge/assets/140991773/255581cf-564e-430b-831b-fea0720ffd73"> and <img width="113" alt="Screenshot 2023-10-17 at 1 51 10 PM" src="https://github.com/wsylliac/matplotlib-challenge/assets/140991773/d3062206-639b-4702-bc1f-7a191c437d10"> DataFrames into a single DataFrame.
2. Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned   DataFrame for the remaining steps.
3. Display the updated number of unique mice IDs.

## Generate Summary Statistics

Create a DataFrame of summary statistics. Remember, there is more than one method to produce the results you're after, so the method you use is less important than the result.

Your summary statistics should include:
* A row for each drug regimen. These regimen names should be contained in the index column.
* A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

## Create Bar Charts and Pie Charts

1. Generate two bar charts. Both charts should be identical and show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.

      * Create the first bar chart with the <img width="132" alt="Screenshot 2023-10-17 at 2 02 31 PM" src="https://github.com/wsylliac/matplotlib-challenge/assets/140991773/b6faf8a7-8f5a-4e4b-b4d6-7dfbf6facc52"> method.
      * Create the second bar chart with Matplotlib's <img width="62" alt="Screenshot 2023-10-17 at 2 03 07 PM" src="https://github.com/wsylliac/matplotlib-challenge/assets/140991773/5ef3df04-06a6-4fb8-9949-09cb80f553cb">
methods.

2. Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

      * Create the first pie chart with the Pandas <img width="127" alt="Screenshot 2023-10-17 at 2 03 58 PM" src="https://github.com/wsylliac/matplotlib-challenge/assets/140991773/5b4fffba-0d34-4a0f-9ce8-31b5e06282d5"> method.
      * Create the second pie chart with Matplotlib's <img width="61" alt="Screenshot 2023-10-17 at 2 04 28 PM" src="https://github.com/wsylliac/matplotlib-challenge/assets/140991773/a922c23b-db78-452f-8984-65f7dc9aaf77"> methods.

## Calculate Quartiles, Find Outliers, and Create a Box Plot

1. Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:
   
      * Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.
      * Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.
      * Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.
      * Determine outliers by using the upper and lower bounds, and then print the results.

2. Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.

**hint**: All four box plots should be within the same figure. Use this [Matplotlib documentation page](https://matplotlib.org/gallery/pyplots/boxplot_demo_pyplot.html#sphx-glr-gallery-pyplots-boxplot-demo-pyplot-py) 📁 for help with changing the style of the outliers.

## Create a Line Plot and a Scatter Plot

1. Select a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.
2. Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

## Calculate Correlation and Regression

1. Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.
2. Plot the linear regression model on top of the previous scatter plot.
  
