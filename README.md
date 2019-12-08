# Project: Python Data Visualization

The primiart purpose of this project was to identify pull factors of immigration to Canada. I mainly considered data from the world bank as a reliable data source for this project.

# Data Set
# API
One of the main targets of this project was to retrieve data through an Application Programming Interface. We found a data portal to retrieve the data needed for the project. The data received in JSON format, and I created a function to traverse the dictionary to create a table out of it.

Code snippet of the recursive algorithm

![Recursive Algorithm](/Screenshots/recursivealogorithm.png)

This algorithm generates a dictionaroy for each response from  World Bank data API call. Then it is just a matter of converting each dictionary to pandas data frame.

![Output Table](/Screenshots/table.png)
