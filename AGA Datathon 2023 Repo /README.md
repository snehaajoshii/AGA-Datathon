# Marymount 
All our files and commits will be uploaded here.
# Introduction of the members
Himadri Bhandari  
Manuel Gaunaurd  
Meharban Arora  
Sneha Joshi  
Tsiorisoa Rakotondrabe  

# Question
How is graduation rates being affected by federal funds, number of patents (and other innovation indicators), and unemployment rates categorized by state considering the racial differences within each state? 

# Abstract  
This project aims to understand the effect of federal funds, number of patents (and other innovation indicators), and population of unemployed people has on graduation rates considering the racial differences in each state throughout a timeline of 2000-2020. As per our hypothesis, we are expecting a positive relationship between graduation rates and all of our variables, but we will be using regression analysis to understand the effect better. We will also be looking at the summary statistics on each of these variables to understand the nature and differing values within each values. Along with that, we will be working with the summary statistics and relative differences between racial diversity within states to see if it has any effect on any of the above listed variables. The tools we will be mainly using for data analysis will be Python and its open source packages and Google Sheets.  

# Documentation
As a team, we decided that we will be using Google sheets for preliminary organizing of data, then will be using python and its libraries for database creation, data analysis, and visualizations.    

# File description  
The purpose of this section is to make the files and its contents understandable for whoever sees this GitHub.  
Member info.xlsx is a file containing the information for all members of the team.  
Marymount Datathon Abstract is our main document that contains our abstract.  
RegressAll.ipynb is our Jupyter notebook where we did visualizations and regressions for all the data points using libraries within python such as pandas, numby, scipy.stats, seaborn, and matplotlib.
RegressSelective.ipynb is our Jupyter notebook where we did visualizations and regressions for all the data points except West Virginia using libraries mentioned above. West Virginia was removed to understand the relationship each of the variable had with graduation rates after considering the outlier as a special case as it was an outlier in the graduation rates.  

# Data Extracting
All the links to our data sources have been added to the folder called "Data links" within our repository "Marymount".  
The links that have been used as shown in the file are given below:  
1. Data for employment rates:  
https://www.bls.gov/lau/ex14tables.htm     
Downloaded data in Google Sheets: https://docs.google.com/spreadsheets/d/e/2PACX-1vQW1kmMZiVy15ra62WagVI9Krb3P2MUfn-rsttKsjp7GVgXXj830teB3WVwOW8S7TcFcLcV6YeuSBtJ/pubhtml     
Cleaned data in Google sheets: https://docs.google.com/spreadsheets/d/e/2PACX-1vTsIxE1aJPKD3sAILw9Vmr98bZPSo7n6grRs09wfeatoHoa0A2C3gpK7Nm_wlL5R61CShl6ObU0rvvm/pubhtml

     Procedures used in organizing data using Google Sheets:  
   While looking at the data for unemployment and employment rates per state per ethnic/racial groups, we found several subcategories to many ethnicities and race, which we wanted to filter out. To explain this better, an example of this was the categorization of a race's males into different age groups as we can see in the original data that has been extracted. But we removed the subcategories of age group for each race and included the total number of employed and non-employed populations within a state by race per year.  
   To do that, firstly, column D was highlighted, and data was looked upon using the function Find and Replace. We put in the exact words for the subcategories like "White women, 15-24 years", "White women, 25-30 years", "Black men, 25-30 years", "Asian men, 25-30 years" etc. and replaced it with blanks. Then we looked at all the blanks in the column D, and deleted rows for all of those rows which had a blank value for column D manually.
   For the merging of data, we used manual data entry for column E and F, and used the function of VLOOKUP to merge data for column G and H (referring to the "Final Merged data for datathon" file in google sheets).
   
3. Data for the number of students that graduated on time:  
https://nscresearchcenter.org/wp-content/uploads/CompletingCollegeAppendix2021.xlsx
4. Data for the number of patents awarded per state per year to people working in Science and Engineering:      
https://ncses.nsf.gov/indicators/states/indicator/patents-per-1000-se-occupation-holders    
5. Data for the federal funding obligated in each state:  
https://ncses.nsf.gov/indicators/states/indicator/federal-rd-obligations-per-se-occupation-holder
6. Data for the demographics of each state:
https://www.kff.org/other/state-indicator/distribution-by-raceethnicity/?dataView=1&currentTimeframe=0&selectedRows=%7B%22states%22:%7B%22all%22:%7B%7D%7D,%22wrapups%22:%7B%22united-states%22:%7B%7D%7D%7D&sortModel=%7B%22colId%22:%22Location%22,%22sort%22:%22asc%22%7D


# Statistical Modeling  
We have used the following statistical tools in order to understand and analyze the data better:    
a. Descriptive statistics  
b. Multilinear regression  
c. Statistical significance  
  
# Data Visualizations  
 For data visualizations, we have used visualizations like:  
a. Scatterplot  
b. Stacked Chart   
c. Bar Chart  

Data Visualizations are done using two different tools namely: Google Sheets and Python.   
1. Federal R&D Obligations per individual per state throughout years in S&E occupation: We created a stacked bar chart showing the differences in the funding obligation per individuals in S&E occupation in each state. The link to the sheet is given below:   
   https://docs.google.com/spreadsheets/d/e/2PACX-1vSHsB6wEoHQ1yF-HeUuE0A2pu8sVEJrsc2Ev7naqITvOdDEOM9jK_LDLugyOhK66cW6bVtmARAmA9hJ/pubhtml
2. Number of patents developed in each state over time: We created a stacked bar chart showing the registered number of patents from the sector of S&E per 1000 individuals in each state. The link for the visualized data is given below:  
https://docs.google.com/spreadsheets/d/e/2PACX-1vTzn9fmx3J9mfMhpE2OfKemn6Ai0BUdGCAqIoCcxk_n_DFftMku8UOn9eKgI1WggUIOAXyip3YhO2Rz/pubhtml
3. Graduation rates categorized by ethnicity per state: We created a categorized bar chart to show how graduation rates differ between ethnicities categorized by state: https://docs.google.com/spreadsheets/d/e/2PACX-1vSujS1TAblhaLrsyuX-qDlfCdelzRetGK3ZfF9pIk-iEIy91NUgaAJM5Z54CnslqTg5_PAtrEHr4OQX/pubhtml
4. Demographics data analysis and visualizations: https://docs.google.com/spreadsheets/d/e/2PACX-1vR80umTMrhg6VvyB0A_tYKbl_IsvBMx4i5gq1XLNkGohPSlzS29p-hkzOW21gw6fcjD7ZGb1zvfS0rU/pubhtml 
While the links to all the google sheets have been put up in the folder of Data Links, the regression and visualizations done on Python has been done on the different files of python.     

# Interpretation  
According to the regression analysis done in the python file named "RegressionAll.ipynb", some of the interpretations that can be made are:  
The first regression in the program shows the relationship between graduation rate and unemployed people per state throughout the years. It shows that they have  a negative relationship where the graduation rate is expected to increase by approximately 0.00062% when the unemployed person per state increases by 1 person.   
  
The second regression shows the relationship between Patents Awarded and Graduation Rate. This shows that there is a positive relationship between patents awarded to individuals where an increase of one thousand patents awarded in Science and Engineering per state approximately increases the graduation rate by 0.073380%.With R-squared being 0.050590, we can say that 5% of the variation in graduation rate is explained by the variable patents awarded per state in Science and Engineering occupations. With the p-value being 0.000015, which is much less than 0.05, we can say that this relationship shown by the regression is statistically significant.  
  
The third regression shows the relationship between Research and Development Obligations per individuals in Science and Engineering Occupations and Graduation Rate. This shows that there is a positive relationship between patents awarded to individuals where an increase of one dollar of Research and Development Obligation per individual worker in Science and Engineering per state approximately decreases the graduation rate by 0.000006%. With R-squared being 0.001310, we can say that 0.13% of the variation in graduation rate is explained by the variable Research and Development Obligation per individual worker in Science and Engineering per state. With the p-value being 0.491170, which is slightly less than 0.05, we can say that this relationship shown by the regression is statistically significant.  

  Multilinear regression analysis:  
  We performed a multilinear regression. Here we are looking at the relationship each variable has with the graduation rates by controlling for other variables. We can see that among the variables, federal funding is not statitically significant when relating to the effect it has on graduation rates. An increase of patents awarded per 1000 people in S&E approximately increases the graduation rate by 0.0845%. An increase of unemployed people per state by 1 person, the graduation rate is assumed to decrease by 0.0013%. Both of these values for relationship have a statistical significant value.
  
According to the regression analysis done in the python file named "RegressionSelective(1).ipynb", some of the interpretations that can be made are:
The above program shows the relationship between graduation rate and unemployed people per state throughout the years except West Virginia. It shows that they have a negative relationship where the graduation rate is expected to decrease by approximately 0.000875% when the unemployed person per state increases by 1 person. With R-squared being 0.013243, we can say that 1.3% of the variation in graduation rate is explained by the variable unemployed people per state. With the p-value being 0.029026, which is less than 0.05, we can say that this relationship shown by the regression is statistically significant.
  
The second regression shows the relationship between between Patents Awarded and Graduation Rate excluding the outlier for West Virginia. This shows that there is a positive relationship between patents awarded to individuals where an increase of one thousand patents awarded in Science and Engineering per state approximately increases the graduation rate by 0.059267%.With R-squared being 0.057851, we can say that 5.7% of the variation in graduation rate is explained by the variable patents awarded per state in Science and Engineering occupations. With the p-value being 0.000004, which is much less than 0.05, we can say that this relationship shown by the regression is statistically significant.  

The third regression shows the relationship between Research and Development Obligations per individuals in Science and Engineering Occupations and Graduation Rate. This shows that there is a negative relationship between patents awarded to individuals where an increase of one dollar of Research and Development Obligation per individual worker in Science and Engineering per state approximately decreases the graduation rate by 0.000007%. With R-squared being 0.003850, we can say that 0.38% of the variation in graduation rate is explained by the variable Research and Development Obligation per individual worker in Science and Engineering per state. With the p-value being 0.240261, which is greater than 0.05, we can say that this relationship shown by the regression is statistically significant.  

  Multilinear regression:  
  We performed a multilinear regression. Here we are looking at the relationship each variable has with the graduation rates by controlling for other variables after omitting West Virginia as it was an outlier. We can see that among the variables, federal funding is not statistically significant when relating to the effect it has on graduation rates. An increase of patents awarded per 1000 people in S&E approximately increases the graduation rate by 0.0708%. An increase of unemployed people per state by 1 person, the graduation rate is assumed to decrease by 0.0014%. Both of these values for relationship have a statistical significant value.

  ##Alternative Analysis

Our findings on the relationshpip between graduation rate and federal funds, number of patents, and unemployment rates categorized by state considering the racial differences within each state was inconclusive. None of the regression models explained the evolution of graduation rate with satisfying significance. However, when looking at the relationship between our datasets, some relations revealed themselves.

![image](https://github.com/AGA-Datathon-2023/Marymount/assets/147752634/c1e82176-f9dc-488b-84aa-cdba4c27def7)

The visualisation above showcases a correlation heatmap of all the numerical variables of our datasets. The Research and Development related variables are highly correlated with each other, seen on the bottom right corner. The variable that seem to have an interesting relation with our Federal R&D variables is the overall number of employed. The variables with high correlation coefficient are the civil non-institutionalized population,  number of patents awarded, number of foreign-born in Science and Engineering, all workers in science and engineering, R&D performed, and state GDP. This triggered a new set of investigation aimed at explaining these high correlation coefficients. 

When breaking down the number data on labor force and completion rates by race, the same overall pattern shows on the correlation matrix but with different intensities. The data related to the white demography is the closest to the aggregate data and the black demography seems to be the pallest on quick look. 

![image](https://github.com/AGA-Datathon-2023/Marymount/assets/147752634/ffc8a08d-0405-420a-8dd0-070cbb6b39a1)

Further analysis was done through multivariate regression. Four analysis were made by creating a model based on the high coefficient rate bivariate, each is done with a filter to categorize race in our master dataset. Each model gave information on the relationship between Federal R&D related variables and employment number for each race. 
 - White: r-squared and adjusted r-squared are over 0.9, with p-values <0.05 for each predictor.
 - Black: The model does not use the variables the other race categories do. The research related variables are not considered to be statistically significant for black employment number.
 - Hispanic: adjusted r-squared over 0.9 with all the variables listed as good predictors except for non-instititionalized civilian population.
 - Asian: r-squared = 0.645 and adjusted r-squared are 0.644, with p-values <0.05 for each predictor.


# Results
Upon looking at the regressions done with Python, we can conclude that as unemployed person per state increases by 1 person, the graduation rates are expected to increase by approximately 0.00062. Additionally, we also conclude that an increase of one thousand patents awarded in Science and Engineering per state approximately increases the graduation rate by 0.073380%. Lastly, our third regression shows us that an increase of one dollar of Research and Development Obligation per individual worker in Science and Engineering per state approximately decreases the graduation rate by 0.000006%. These are interesting and relevant findings as they show us how different independent variables (as mentioned above) each effect the graduation rates in the United States. 

We also conducted a multi linear regression where we saw how much of the graduation rates is explained by each of our independent variables. With R-squared value being 0.013243, we can say that 1.3% of the variation in graduation rate is explained by the variable unemployed people per state. With R-squared being 0.057851, we can say that 5.7% of the variation in graduation rate is explained by the variable patents awarded per state in Science and Engineering occupations. With R-squared being 0.003850, we can say that 0.38% of the variation in graduation rate is explained by the variable Research and Development Obligation per individual worker in Science and Engineering per state. For our first two variables (Unemployed People and Patents Awarded) the p-value is less than 0.05 indicating that they are statistically significant at the 95% level, on the other hand, the variable Research and Development Obligation is not statistically significant at the 95% level as the p value is greater than 0.05.

We also looked into demographics per state per year and what conclusions can we draw from that data. We created data visualizations to see the distribution of ethnicities in all states throughout the years. We then looked at each ethnicity individually by state throughout the years. In some states, we observed certain ethnicities having a larger population than other states. For example, we observed that the Hispanic population in the state of Colorado was the largest among all the other states, followed by Texas throughout the years. We did have one outlier, the state of West Virginia, and we decided to create two different sets to see the difference between the set that includes the outlier and one that does not include the outlier. We observed that when we remove the outlier (West Virginia), we get a consistent trend between all the other states in repsect to our variables. When we look at the visualizations for demographics per state, we can understand how ethnicities play a role in all states in the US with repsect to our variables in question and if there is a connection between ethnicities in states and the funding within states.

We observe that the civil non-institutionalized population, number of patents awarded, number of foreign-born in Science and Engineering, all workers in science and engineering, R&D performed, and state GDP can be used to predict the number of employed with modeling from data from each state and split by year for model training. Each model categorized by race give insight on the relationship between the employed by race and federal research efforts.

# Licenses
