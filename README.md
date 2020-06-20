DATA QUESTION 3: Analysis of Earthquakes from Historical Data

Goals for the project:
1) Extract historical earthquake data using webscraping and load the data
2) Preprocess data for data analysis
3) Explanatory data analysis

Tools Used:
1) Python-Pandas library
2) Webscraping- BeautifulSoup
3) Regular Expressions

DATASET USED:
https://en.wikipedia.org/wiki/List_of_deadly_earthquakes_since_1900 

Data cleaning tasks include:

Replace empty strings with NaN
Remove the footnotes from the 'Other Source Deaths' column
Convert Magnitude to numeric
Correct number of deaths when there is more than one value. When there is more than one value given, choose the largest.
Create a new column ('deaths') that evaluates the four total-death columns ('PDE Total Deaths', 'Utsu Total Deaths', 'EM-DAT Total Deaths', and 'Other Source Deaths') and populates the new column with the highest value.
Explore the data in terms of when and where earthquakes occurred and how severe they were (magnitude, deaths, secondary effects).


Questions Pondered:

Part 1:
Nate Silver discusses the difficulty of predicting earthquakes in The Signal and the Noise. Nevertheless, we will try to identify some patterns by analyzing the deadly earthquakes that have occurred since 1900.

The table of earthquakes from https://en.wikipedia.org/wiki/List_of_deadly_earthquakes_since_1900 were imported using the requests and beautifulsoup library and loaded onto a pandas dataframe. 


Are there factors that make an earthquake more likely?
Are there factors that make an earthquake more deadly?
Where would you live if you wanted to eliminate the risk of experiencing a deadly earthquake? Where would you avoid living?


Part 2:
Use the requests library and the USGS's API (https://earthquake.usgs.gov/fdsnws/event/1/) to retrieve information about all recorded earthquakes that occurred in Tennessee since 1900. 

Questions answered for Tennessee:

How many earthquakes are in the dataset? Which region of Tennessee seems to be the most prone to earthquakes? Which is the least prone?
Do the magnitudes of earthquakes seem to follow the distribution described by Nate Silver. That is, one higher magnitude is ten times less likely to occur?
How worried do Tennesseans need to be about a deadly earthquake striking? What about Nashvillians?
