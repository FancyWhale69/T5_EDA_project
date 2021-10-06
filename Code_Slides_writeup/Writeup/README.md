# Predicting Crowded stations in Riyadh's Metro
Hazim Bukhari

## Abstract
The aim of the project is to predict which stations are most likely to be crowded in Riyadh to foucs on them in future plans. The data is extracted from the [MTA](http://web.mta.info/developers/turnstile.html) from Jan 2020 until Dec 2020. Crowded stations will be identified in the MTA dataset then extracting thier land use, and finally mapped to Riyadh's metro stations. Results will be shared via Power point slides and Blog post (in progress).

## Design
This project originates from the [DrivenData competition](https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/) "Pump it Up: Data Mining the Water Table". The data is provided by [Taarifa](http://taarifa.org/) and the Tanzanian Ministry of Water, and presents a three-class operational status of **functional**, **functional needs repair**, and **non-functional** for waterpoints across the country. Classifying statuses accurately via machine learning models would enable the Tanzanian Ministry of Water to take action to improve operations and maintenance planning of these units, allocate resources more quickly to needed areas, and ensure potable water is accessible to as many people as possible.

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


