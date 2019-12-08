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
