# Project: Python Data Visualization

The primiart purpose of this project was to identify pull factors of immigration to Canada. I mainly considered data from the world bank as a reliable data source for this project.

# Data Set
## API
One of the main targets of this project was to retrieve data through an Application Programming Interface. We found a data portal to retrieve the data needed for the project. The data received in JSON format, and I created a function to traverse the dictionary to create a table out of it.

Code snippet of the recursive algorithm

![Recursive Algorithm](/Screenshots/recursivealogorithm.png)

This algorithm generates a dictionaroy for each response from  World Bank data API call. Then it is just a matter of converting each dictionary to pandas data frame.

![Output Table](/Screenshots/table.png)

# Data Analysis

We considered following pull factors for analysis of this project, and we retrived data for each factor from World Bank data API and ran against the above recursive alogorithm to generate pandas data frames.

  - Top 3 countries of immigrants
  - Poplulation
  - Gross Domestic Product (GDP)
  - Consumer Price Index (CPI)
  - Unemployment
  - Employment

## Analysis 1 - Number of immigrants
  - based on a 10 year data set from 2008 - 2017, clearly shows a significant increase of immigrants during 2009 - 2011, and then again from 2015.
  - it is intersting to know the year **2011** had the lowest number of immigrants

![No of Immigrants](/Screenshots/noofimmigrants.png)

## Analysis 2 - Top 3 Provinces with most Immigrants
  - It proved to be Alberta had most immigrants in Canada followed by Ontratio, and British Columbia
  
  ![Heatmap](/Screenshots/heatmap.png)

## Analysis 3 - Top 3 Countries with most migration to Canada
  - China
  - India
  - Philippines
  
  ![top3countries](/Screenshots/top3countries.png)
  
## Analysis 4 - Population Demographics
  ![PopulationDemographics](/Screenshots/PopulationDemographics.png)

## Analysis 5 - Consumer Price Index
  ![cpi](/Screenshots/cpi.png)
  
## Analysis 6 - Gross Dosmestic Product Hypothesis
  - **GDP** is the one of the most common indicators used to track the health of a nation's economy. It inclues a number of dofferent fators such as consumption and investment over a period of time.
  - H0: μ1 = μ2 = μ3 = μ4
  - H1: The means are not all equal
  
  ** Boxplot grouped by country (GDP %)**
  - The p value from the anova test rejects the null hypothesis. All the 4 countries do not have a similar GDP as pvalue is greater than .10. Therefore the average GDP rise is not the same. In fact there is a great difference amonth the GDP values of the 4 countries.
  - pvalue 3.578779945786309e-11
  
  ![GDP-Boxplot](/Screenshots/GDP-Boxplot.png)
    
  - China shows a consistent increase in GDP between 2009 to 2018
  - Canada GDP is not only significantly lower than China it is even lower than India between 2015 to 2018
  - It explains why we reject null hypothesis as the GDP per year is significantly differenent

## Analysis 7 - Unemployment
  - Canada tends to have a higher unemployment rate in comparison to the top 3 immigrant countries
  - Primary reason was GFC in 2009 & secondly China and India have roughly 20 times bigger economy which created more opportunities resulting less Unemployment rate
  ![unemployment4countries](/Screenshots/unemployment4countries.png)
  
## Analysis 8 - Employment
  - China and India dominated the Total population stats in Billions, in Contrast Canada still stuck below 40 million even at 2018
  - Having total Population below 40 Million was literally a “Blessing in disguise” for Canada
  - Employment to population ratio is around 62.5% whereas India is just around 50% mark 
![employment](/Screenshots/employment.png)
  
# Conclusion
  - Aging population has been increasing fast while young people are not increasing at the same pace. This might create an imbalance in the retirement pension. 
  - Temporary worker and Permanent Resident fulfil this GAP in retirement pension.
  - Some reasons that Canada is attractive:
    - GDP has been increasing
    - Low rate of unemployment and an increased rate of employment
    - CPI shows  that is the inflation is under control 
    - Big continent but  with small number of people

**Initiation of this project led me creating the resursive alorithm that can travse  python dictionaries to create data frames automatically.**
