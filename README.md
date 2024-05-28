![image](https://github.com/ngauthu/gapminderCO2/assets/20643257/72f9e416-eda4-41bc-bca1-095915a80801)# Gapminder-CO2-analysis
Visualization of CO2 emission across countries and any potential correlations

## Dataset overview

> About data provider Gapminder: Gapminder has collected a lot of information about how people live their lives in different countries, tracked across the years, and on a number of different indicators. The data used can be downloaded from Gapminder [here](https://www.gapminder.org/data/).


For this project, CO2 emission per person was collected between 1998 and 2017 together with GDP per capita (inflation-adjusted), broadband subscribers per 100 people, freedom index, industry percent in GDP, agricultural percent in GDP. Each indicator is stored in a separate excel spreadsheet downloaded on 23rd March 2022. These indicators are merged together in one full dataset.



## Summary of analysis

The 2 core questions I aim to answer for this project are:

> Question 1: Is the average CO2 per person going up or down between 1998 and 2017? Are there any differences among the continents?

Between 1998 and 2017, the overall world trend is steadily increasing. CO2 per person in Europe, Asia and North America on average are higher than average CO2 per person in all 156 countries, while average CO2 per person in South America, Oceania and Africa are lower than average Co2 per person in all 156 countries. CO2 per person in Europe is on a more noticeable downward trend since 2008, as compared with that in other regions.

> Question 2: Are there any possible correlations found between the CO2 emission per person and other indexes including the GDP per capita, number of broadband subscribers per 100 people, freedom index, percentage of industry contribution to the GDP, and percentage of agriculture contribution to the GDP

GDP per capita seems to have a positive correlation with CO2 emission per person for very developed countries, developed countries and developing countries. We cannot, however, find correlation between CO2 emission per person with freedom index, agriculture percentage in GDP and industry percentage in GDP. Possible areas for further investigation lie in the underdeveloped countries where GDP per capita does not seem to have any correlation with the CO2 emission per person. It could be that there is a certain threshold in GDP per capita that only above this,we can notice a correlation between these 2 indexes.

We might also need a wider time span (repeated findings in multiple years) to confirm the correlations between CO2 emission per person and other indexes. More efforts can also look into confirming if agriculture percentage in GDP and industry percentage in GDP do not have correlation with CO2 emission per capita. We can also try using other indexes to measure CO2, for example, only total CO2 emission or CO2 emission per USD earned in GDP.

## Data wrangling and analysis highlights

> The separate datasets are joined together based on country and year
> We narrow down by countries with 20 years of data available & fill in/ replace some variables to introduce more meaning and structure to the data processing
> As an overview, I created a function to draw histograms on the same axes for different years with input in variable, year and color defined.
> I used this function to summarize the distribution for the numerical variables: CO2 emission per person, GDP per capita, freedom index, industry GDP percent and agriculture GDP
percent
> For the first question, I summarized these same variables as averages per continent and used colored line chart to demonstrate how the averages of different continents vary between 1998 and 2017.
> For the second question, I used scatter plots to look at the correlation between CO2 emission per person and other variables. Another layer to the scatter plots is the grouping of the countries based on the GDP per capita.
