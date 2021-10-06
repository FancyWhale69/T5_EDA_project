# Predicting Crowded stations in Riyadh's Metro
Hazim Bukhari

## Abstract
The aim of the project is to predict which stations are most likely to be crowded in Riyadh to foucs on them in future plans. The data is extracted from the [MTA](http://web.mta.info/developers/turnstile.html) from Jan 2020 until Dec 2020. Crowded stations will be identified in the MTA dataset then extracting thier land use, and finally mapped to Riyadh's metro stations. Results will be shared via Power point slides and Blog post (in progress).

## Design
The Riyadh metro organization is the governing body for the metro project in Riyadh, with such a new project some adjustment, but wouldn’t it be nice to have a map that displays the prediction for high traffic stations in advance to prepare in advance and avoid complications down the road?
By using data from the MTA which is the governing body for the subway system in NY, high traffic stations in NY could identified then extracting features of their locations (e.g.: near working area, school zone, housing area, tourist attraction, etc.…).


## Data
The dataset contains ~10M rows with 12 columns, the most important features are:  
1. C/A,UNIT,SCP combo to identifiy a single turnstyile.  
2. STATION to find out their traffic.
3. DATE, TIME combo to seperate entries/exits.
4. ENTRIES, EXITS to find how many people enter/exit the station.

Some additional data for [NY landuse](https://zola.planning.nyc.gov/#13.33/40.74823/-73.98644).

## Algorithms

1. Get how people entered/exited for each turnstyle.
2. Analyise enter/exit values for anomalies.
3. Find and fix problems with the data.
4. Get crowded stations.
5. Extract theier landuse.
6. Predict which stations will be crowded in Ryiadh. 

## Tools
- SQLAlchemy for loading data
- Pandas for data manipulation
- Plotly for interactive visualizations


## Communication
In addition to the slides a blog post will be post it about the study's findings.


