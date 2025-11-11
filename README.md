# 16th Street BART Plaza Crime Dashboard

Data visualization dashboard tracking crime incidents within 500 feet of the 16th Street BART Station in San Francisco's Mission District.

## Python Notebooks and Raw Data

### `bart_crime_update.ipynb`
Main python script for scraping Crimemapping.com and creating the csv of updated crimes. 

### `bart_crime_viz.ipynb`
This script is responsible for cleaning the main data and creating the aggregated subsets of data that will be fed into Datawrapper or used for D3 viz.

### `bart_crime_updated.csv`
Every Monday, the new crimes + old crimes get saved to this CSV. Raw and not standardised.

### `crime_desc.csv`
Total number of crimes broken down by description. Used to make a table in datawrapper.

### `crime_time.csv`
Total number of crimes broken down by month. Used to make a column chart in datawrapper.

### `crimes_stacked.csv`
Crimes broken down by month and type. Used to make a stacked column chart in datawrapper.

## Other Files

### `index.html`
Main dashboard page that displays all crime data visualizations.

### `cal_map.html`
Interactive calendar heatmap showing daily crime incidents for the last 6 months. 

### `calendar_data.json`
Data file containing daily crime records. Each entry includes:
- `date`: Date in YYYY-MM-DD format
- `count`: Number of incidents that day
- `types`: Array of crime type descriptions

The calendar map will automatically show only the most recent 6 months when new data is added.


## Data Source

Crime data is collected weekly from CrimeMapping.com. BART police report incidents to CrimeMapping.com with a 24-hour lag.


## Mission Local

This project is part of Mission Local's accountability journalism covering San Francisco's Mission District.