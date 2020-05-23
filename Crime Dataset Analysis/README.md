# Analysing the New York City Crime Dataset (alongside a couple of other datasets)

This week, I'm going to be running through an overview of the datasets I was looking at a while ago (the New York City Crime Datasets).
- Previously, I was looking through the crime dataset to predict the number of crime events in future time steps given some prior information. 
- Let's see how I can develop with this, or what tools I can use in an upcoming project soon!

# Chapter 1: Data Overview
Crime Data link:

https://data.cityofnewyork.us/Public-Safety/NYC-crime/qb7u-rbmr

311 Data Link:

https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9

The most relevant datasets in this analysis is the crime and complaints dataset, which was collected around June 2019. The data was cleaned to only include events that happened over 2018 (0:00 1/1/2018 - 0:00 1/1/2019), within one of the five boroughs of New York (Manhattan, Bronx, Brooklyn, Queens, and Staten Island). These geographical boundaries were defined by the geo files from New York Open data. 

To do:
- Maybe brief overview of Uber data,
- Brief overview of Weather data
- Brief overview of Demographic data


## 311 Complaints

| 311 Type 	| Original 311 Categories 	| # Events 	| # Events (3 boros) |
|---------------	|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------	|---------------------:	|
| Noise 	| ‘Noise’, ‘Noise – House of Worship’, ‘Noise – Park’, ‘Noise – Helicopter’ , ‘Noise – Vehicle’,  ‘Illegal Fireworks’, ‘Noise – Street/Sidewalk’, ‘Noise – Commercial’ , ‘Noise – Residential’ 	| 345,828 	| 32,762 |
| Infringements 	| ‘Disorderly Youth’, ‘Emergency Response Team (ERT)’, ‘Public Assembly – Temporary’,  ‘Investigations and Discipline’, ‘Other Enforcement’, ‘Drug Activity’, ‘Drinking’,  ‘Urinating in Public’ , Blocked Driveway’, ‘Illegal Parking’ 	| 257,712 	| 17,040 |
| Street Damage 	| ‘Abandoned Vehicle’, ‘Scaffold Safety’, ‘Bridge Condition’, ‘Non-Residential Heat’,  ‘Street Sign – Dangling’, ‘Highway Sign – Dangling’, ‘Highway Sign – Damaged’,  ‘Street Sign – Missing’, ‘Street Sign – Damaged’, ‘Broken Parking Meter’ 	| 24,583 	| 1,497 |
| Cleanliness 	| ‘Building Condition’, ‘Unsanitary’, ‘Overflowing Recycling Baskets’,  ‘Recycling Enforcement’, ‘Beach/Pool/Sauna Complaint’, ‘Industrial Waste’,  ‘Unsanitary Animal Facility’, ‘Graffiti’, ‘Litter Basket / Request’, ‘Mold’,  ‘Sweeping/Missed’, ‘Sanitation Condition’, ‘Roof/Sewer/Sidewalk Condition’,  ‘Overflowing Litter Baskets’, ‘Sidewalk Condition’, ‘Street Light Condition’,  ‘Dirty Conditions’, ‘Air Quality’, ‘Derelict Vehicles’, ‘Street Condition’,  ‘Curb Condition’, ‘Traffic Signal Condition’, ‘UNSANITARY CONDITION’, ‘Derelict Vehicle’ 	| 375,503 	| 22,426 |
| Environment 	| ‘Plant’, ‘Snow’, ‘Violation of Park Rules’, ‘Illegal Tree Damage’,  ‘Overgrown Tree/Branches’, ‘Damaged Tree’, ‘Sewer’ 	| 82,824 	| 4,409 |

## NYC Crime Data

# Chapter 2: Map of New York City + Uber Movement Data
New York is separated into five boroughs, and further separated into 194 different Neighbourhood Tabulation Areas (NTAs). We use this map 

https://movement.uber.com/?lang=en-AU

# Chapter 3: New York Crime/Complaint Data


# Chapter 4: New York City Demographic Data


# Chapter 5: New York City Weather Data


# Chapter 6: New York City Public Transport Data


# Chapter 7: Other Datasets


# Appendix
Right now, I've set this as a general EDA for all 6(?) datasets, but this might change depending on how things will go. 

### List of datasets:
- NYC Crime Datasets (from NYC Open Data)
- NYC Complaint Datasets
- NYC Weather Dataset (from Weather Underground)
- NYC MTA Datasets (from MTA)
- NYC Uber Network Data
- NYC Camera Feed Data(?)

[__Back to the main page__](https://phillipluong.github.io/PyTorchProjects101/)
