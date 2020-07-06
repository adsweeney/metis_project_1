## Objective:
Optimize placement of street teams around MTA train stations. 

## Data:
- [MTA Turnstile Data](http://web.mta.info/developers/turnstile.html) 
- [NYCHealth COVID Data](https://github.com/nychealth/coronavirus-data)

# Code:

2 files, DataFunctionsFinal and Maps_2

DataFunctionsFinal deals with data gathering and processing. Maps_2 deals with graphing data onto maps.

## DataFunctionsFinal
[DataFunctionsFinal](https://github.com/adsweeney/metis_project_1/blob/master/DataFunctionsFinal.ipynb) contains functions that cleans, processes data for usage, and generates plots.

### Has functions 

clean : takes in list of weeks and returns cleaned dataframe with data from MTA

get_counts_entry/exit : adds columns that track deltas for exits. Also has a timecop function that keeps track of temporal inconsistencies.

turnstile : function that calls other functions in order to return a workable dataframe in order to be plotted

### Has separate code
'top'  - code to find and list the top targets based on traffic

'translate' - code that translates "Remote Unite" codes into station names, based on the frequency of the station name showing up in relation to the Remote Unit.

'prettyplot' - a set of code to create extra visualizations and changed scales for the dataframe stored in memory after running turnstile

'font visualizer' - code to run in Jupyter notebook to check what fonts are avaiable

and other debug code

## Maps 2
[Maps 2](https://github.com/adsweeney/metis_project_1/blob/master/Maps%202.ipynb) contains code for mapping stations and COVID choropleth map. 
