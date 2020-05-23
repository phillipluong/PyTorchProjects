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

| Crime Type | Original Crime Categories | # Events | # Events (3 boros) |
|-------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:------------------|:------------------|
| Assault | ‘assault 3 & related offenses’, ‘felony assault’, ‘murder & non-negl. manslaughter’, ‘homicide-negligent, unclassifie’, ‘homicide-negligent-vehicle’ | 73,280 | 4,328 |
| Drug | ‘dangerous drugs’, ‘alcoholic beverage control law’ | 15,262 | 649 |
| Harrassment | ‘harrassment 2’ | 69,289 | 3,876 |
| Larceny | ‘petit larceny’, ‘grand larceny’, ‘robbery’, ‘burglary’, ‘grand larceny of motor vehicle’, ‘theft-fraud’, other offenses related to thef’, ‘theft of services’, ‘petit larceny of motor vehicle’, ‘jostling’ | 161,063 | 9,503 |
| Traffic | ‘vehicle and traffic laws’, ‘intoxicated & impaired driving’, ‘intoxicated/impaired driving’ | 11,667 | 581 |

# Chapter 2: Map of New York City + Uber Movement Data
New York is separated into five boroughs, and further separated into 194 different Neighbourhood Tabulation Areas (NTAs). We use this map 

https://movement.uber.com/?lang=en-AU

| Month     | Data Points | Unique Nodes | Unique Edges |
|-----------|:-------------:|:--------------:|--------------:|
| January   |  15,945,242 | 51,226       | 64,888       |
| February  |  15,017,889 | 50,369       | 63,350       |
| March     |  18,083,045 | 52,976       | 68,007       |
| April     |  17,201,955 | 52,790       | 65,946       |
| May       |  18,612,705 | 53,654       | 68,878       |
| June      |  40,076,432 | 55,280       | 73,363       |
| July      |  19,035,601 | 53,244       | 68,554       |
| August    |   2,575,901 | 12,882       |  9,040       |
| September |  17,837,387 | 53,753       | 68,867       |
| October   |  18,073,444 | 53,309       | 68,295       |
| November  |  16,244,698 | 53,346       | 68,181       |
| December  |  15,949,334 | 51,822       | 65,104       |
| Total     | 214,653,633 | 58,299       | 78,660       |

# Chapter 3: New York Crime/Complaint Data


# Chapter 4: New York City Demographic Data

| _Economic_                | _Housing_       |
|---------------------------|-----------------|
| Class of Worker           | # Bedrooms      |
| Employment Status         | Gross Rent      |
| Health Insurance Coverage | Heating         |
| Income + Benefits         | Monthly Costs   |
| Industry                  | Mortgage status |
| Occupation                | Occupancy       |
| _Populational Diversity_  | Owner Costs     |
| Race                      | # Rooms         |
| Sex                       | Tenure          |
| Age                       | Total # Units   |
|                           | Value per unit  |
|                           | # Vehicles      |

# Chapter 5: New York City Foursquare Data
| Time Period | Time Period       | Number of Hours |
|-------------|:-------------------|-----------------:|
| Morning     |  6:00am –  9:59am | 4               |
| Midday      | 10:00am –  2:59pm | 5               |
| Afternoon   |  3:00pm –  6:59pm | 4               |
| Night       |  7:00pm – 11:59pm | 5               |
| Overnight   | 12:00am –  5:59am | 6               |

# Chapter 6: New York City Weather Data


# Chapter 7: New York City Public Transport Data


# Chapter 8: Other Datasets


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
