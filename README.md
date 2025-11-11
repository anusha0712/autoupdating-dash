# 16th Street BART Plaza Crime Dashboard

Data visualization dashboard tracking crime incidents within 500 feet of the 16th Street BART Station in San Francisco's Mission District.

## Python Notebooks and Raw Data

1. `bart_crime_update.ipynb`
Main python script for scraping Crimemapping.com and creating the csv of updated crimes. 

2. `bart_crime_viz.ipynb`
This script is responsible for cleaning the main data and creating the aggregated subsets of data that will be fed into Datawrapper or used for D3 viz.

3. `bart_crime_updated.csv`
Every Monday, the new crimes + old crimes get saved to this CSV. Raw and not standardised.

4. `crime_desc.csv`
Total number of crimes broken down by description. Used to make a table in datawrapper.

5. `crime_time.csv`
Total number of crimes broken down by month. Used to make a column chart in datawrapper.

6. `crimes_stacked.csv`
Crimes broken down by month and type. Used to make a stacked column chart in datawrapper.

## Other Files

1. `index.html`
Main dashboard page that displays all crime data visualizations.

2. `cal_map.html`
Interactive calendar heatmap showing daily crime incidents for the last 6 months. 

3. `calendar_data.json`
Data file containing daily crime records. Each entry includes:
- `date`: Date in YYYY-MM-DD format
- `count`: Number of incidents that day
- `types`: Array of crime type descriptions

The calendar map will automatically show only the most recent 6 months when new data is added.


## Data Source

Crime data is collected weekly from CrimeMapping.com. BART police report incidents to CrimeMapping.com with a 24-hour lag.


## Mission Local

This project is part of Mission Local's accountability journalism covering San Francisco's Mission District.